cmake_minimum_required(VERSION 2.8.3)
project(ngws_gazebo)

find_package(catkin REQUIRED)

catkin_package()

#catkin_add_env_hooks(gazebo_setup SHELLS bash DIRECTORY #${CMAKE_CURRENT_SOURCE_DIR}/env_hooks)

install(DIRECTORY launch
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

install(DIRECTORY worlds
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
