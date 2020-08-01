cmake_minimum_required(VERSION 3.5)
project(mcl_3dl_msgs)

set(MESSAGE_DEPENDS
  std_msgs
)

find_package(ament_cmake REQUIRED)

find_package(rosidl_default_generators REQUIRED)

rosidl_generate_interfaces(${PROJECT_NAME}
  "msg/Status.msg"
  "srv/ResizeParticle.srv"
)

ament_package()