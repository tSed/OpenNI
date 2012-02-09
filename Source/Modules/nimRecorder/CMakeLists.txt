##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

include_directories(../Common)
qi_create_lib(nimrecorder
  SRC *.h *.cpp ../Common/*.h ../Common/*.cpp
  )
qi_use_lib(nimrecorder
  openni
  )
qi_stage_lib(nimrecorder)
