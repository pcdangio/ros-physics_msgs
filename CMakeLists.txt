cmake_minimum_required(VERSION 3.0.2)
project(physics_msgs)

# Find catkin and package dependencies.
find_package(catkin REQUIRED COMPONENTS
  message_generation)

# Add message files.
add_message_files(
  FILES
  acceleration.msg
  angular_velocity.msg
  velocity.msg)

# Generate messages.
generate_messages()

# Create catkin package.
catkin_package(CATKIN_DEPENDS message_runtime)