##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

# OpenNI guys really do silly things, or at least they don't it in a
# clean way... :'(
#
# They always include Linux-x86/*.h stuff, then override what need to
# be override for the target platform.
#
# So, we have to always install Linux-x86 stuff and add the actual
# target stuff.

set(ARCH_HDRS Linux-x86/*.h)

if("${CMAKE_SYSTEM_PROCESSOR}" MATCHES "arm*")
set(ARCH_HDRS ${ARCH_HDRS} Linux-Arm/*.h)
elseif("${CMAKE_SYSTEM_PROCESSOR}" MATCHES "(i.86|x86_64)")
# already included, do nothing
else()
message(FATAL_ERROR "Unsupported target processor")
endif()

qi_install_header(
  *.h ${ARCH_HDRS}
  SUBFOLDER ni
  KEEP_RELATIVE_PATHS
  )
