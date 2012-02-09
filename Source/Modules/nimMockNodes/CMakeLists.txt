##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

qi_create_lib(nimmocknodes
  SRC *.h *.cpp
  )
qi_use_lib(nimmocknodes
  openni
  )
qi_stage_lib(nimmocknodes)
