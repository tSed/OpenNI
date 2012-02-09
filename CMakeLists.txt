##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

# CMake file for OpenNI
cmake_minimum_required(VERSION 2.8)
project(OpenNI)
find_package(qibuild)

include_directories(Include)
add_subdirectory(Include)
add_subdirectory(Source)
