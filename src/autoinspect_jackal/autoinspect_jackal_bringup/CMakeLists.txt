cmake_minimum_required(VERSION 2.8.3)

project(autoinspect_jackal_bringup)

find_package(catkin REQUIRED COMPONENTS
)

catkin_package(
  INCLUDE_DIRS
  CATKIN_DEPENDS
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)

install(DIRECTORY config launch map rviz DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

