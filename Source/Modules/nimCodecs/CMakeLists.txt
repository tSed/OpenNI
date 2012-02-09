##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

qi_create_lib(nimcodecs
  SRC *.h *.cpp
  )
qi_use_lib(nimcodecs
  openni
  jpeg
  )
qi_stage_lib(nimcodecs)
