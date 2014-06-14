cmake_minimum_required(VERSION 2.8.3)
project(people_detector)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin)
include(ExternalProject)
ExternalProject_Add(people_detector
  SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/people_detector 
  BUILD_COMMAND cd people_detector; make
  INSTALL_COMMAND "")