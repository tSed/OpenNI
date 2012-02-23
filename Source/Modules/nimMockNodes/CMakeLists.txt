##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

qi_create_lib(nimMockNodes
  SRC *.h *.cpp
  )
qi_use_lib(nimMockNodes
  dl
  pthread
  rt
  usb_1
  OpenNI
  )
qi_stage_lib(nimMockNodes)
