##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

qi_create_bin(niLicense
  SRC *.cpp
  )
qi_use_lib(niLicense
  OpenNI
  usb_1
  dl
  )
