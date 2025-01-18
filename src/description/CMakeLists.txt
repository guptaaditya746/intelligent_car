cmake_minimum_required(VERSION 3.5)
project(description)

# Find dependencies
find_package(ament_cmake REQUIRED)
find_package(xacro REQUIRED)
find_package(rviz2 REQUIRED)
find_package(robot_state_publisher REQUIRED)


# Install directories
install(
  DIRECTORY launch rviz urdf ros2_control
  DESTINATION share/${PROJECT_NAME}
)

ament_package()
