# Pinocchio ROS/catkin example [![Build Status](https://travis-ci.com/wxmerkt/pinocchio_ros_example.svg?branch=master)](https://travis-ci.com/wxmerkt/pinocchio_ros_example)

This example demonstrates how to use Pinocchio in a catkin package. Pinocchio is released as a 3rd-party CMake package into ROS Kinetic, Melodic, and Noetic and can be installed using `sudo apt install ros-$ROS_DISTRO-pinocchio`.

To find Pinocchio:
```cmake
find_package(pinocchio REQUIRED)
```

and use:
```cmake
target_link_libraries(${PROJECT_NAME} pinocchio::pinocchio)
```

This example is built on Travis CI for Kinetic, Melodic, and Noetic.
