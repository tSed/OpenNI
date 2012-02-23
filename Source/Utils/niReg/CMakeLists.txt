##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

qi_create_bin(niReg
  SRC *.cpp
  )
qi_use_lib(niReg
  dl
  pthread
  rt
  usb_1
  OpenNI
  )
