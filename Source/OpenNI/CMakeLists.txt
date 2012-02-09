##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

qi_create_lib(openni
  SRC *.h *.cpp Linux/*.h Linux/*.cpp
  )
qi_use_lib(openni
  tinyxml
  usb_1
  )
qi_stage_lib(openni)
