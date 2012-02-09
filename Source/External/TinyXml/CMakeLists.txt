##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

qi_create_lib(tinyxml
  NO_INSTALL
  STATIC
  INTERNAL
  SRC *.h *.cpp
  )
qi_stage_lib(tinyxml)
