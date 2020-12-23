
cmake_minimum_required(VERSION 3.5)
project(rtcm_msgs)

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)
find_package(sensor_msgs REQUIRED)
find_package(std_msgs REQUIRED)
find_package(builtin_interfaces REQUIRED)

rosidl_generate_interfaces(${PROJECT_NAME}
  "msg/RtcmMessage.msg"
  DEPENDENCIES sensor_msgs std_msgs)

ament_package()
