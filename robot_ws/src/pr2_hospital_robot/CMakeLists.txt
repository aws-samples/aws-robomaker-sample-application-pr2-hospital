################################################################################
# Set minimum required version of cmake, project name and compile options
################################################################################
cmake_minimum_required(VERSION 2.8.3)
project(pr2_hospital_robot)

################################################################################
# Find catkin packages and libraries for catkin and system dependencies
################################################################################
find_package(catkin)

################################################################################
# Declare catkin specific configuration to be passed to dependent projects
################################################################################
catkin_package()

################################################################################
# Build
################################################################################
include_directories(
  include
  ${catkin_INCLUDE_DIRS}
)

################################################################################
# Install
################################################################################

install(DIRECTORY launch config
	DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)