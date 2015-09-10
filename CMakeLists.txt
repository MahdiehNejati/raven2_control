cmake_minimum_required(VERSION 2.8.3)
project(raven2_control)

find_package(catkin REQUIRED COMPONENTS
#  ros_control
#  ros_controllers
)

catkin_package()

install(DIRECTORY config
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

install(DIRECTORY launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

include_directories(
  ${catkin_INCLUDE_DIRS}
)

