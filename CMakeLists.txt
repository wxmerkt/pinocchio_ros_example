cmake_minimum_required(VERSION 3.0.2)
project(pinocchio_ros_example)

find_package(catkin REQUIRED)

find_package(pinocchio REQUIRED)
catkin_package()

add_executable(example src/example.cpp)
target_link_libraries(example pinocchio::pinocchio)

install(TARGETS example
  RUNTIME DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
