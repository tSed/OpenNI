##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

if(NOT "${XN_OPEN_NI_FILES_LOCATION}" STREQUAL "")
  add_definitions(-DXN_OPEN_NI_FILES_LOCATION="${XN_OPEN_NI_FILES_LOCATION}")
endif()

qi_create_lib(OpenNI
  SRC *.h *.cpp Linux/*.h Linux/*.cpp
  )
qi_use_lib(OpenNI
  dl
  pthread
  rt
  tinyxml
  usb_1
  )
qi_stage_lib(OpenNI
  PATH_SUFFIXES ni
  DEPENDS dl pthread rt usb_1
  )
