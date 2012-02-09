##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

include_directories(../Common)
qi_create_lib(nimRecorder
  SRC *.h *.cpp ../Common/*.h ../Common/*.cpp
  )
qi_use_lib(nimRecorder
  OpenNI
  )
qi_stage_lib(nimRecorder)
