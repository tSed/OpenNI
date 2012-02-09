##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

qi_create_lib(nimMockNodes
  SRC *.h *.cpp
  )
qi_use_lib(nimMockNodes
  OpenNI
  )
qi_stage_lib(nimMockNodes)
