cmake_minimum_required(VERSION 3.0.2)
project(autoinspect_jackal_description)

find_package(catkin REQUIRED COMPONENTS
)

catkin_package(
  INCLUDE_DIRS
  CATKIN_DEPENDS
)

install(DIRECTORY launch rviz urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

