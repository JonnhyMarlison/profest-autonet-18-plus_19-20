cmake_minimum_required(VERSION 2.8.3)

project(autokin_move_msg)

find_package(catkin REQUIRED COMPONENTS
   std_msgs
   message_generation
)

add_message_files(
   FILES
   autokin_move_msg.msg
 )

generate_messages(
  DEPENDENCIES
  std_msgs
)

catkin_package(
  CATKIN_DEPENDS message_runtime
)

