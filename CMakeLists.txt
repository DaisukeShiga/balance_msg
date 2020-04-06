cmake_minimum_required(VERSION 2.8.3)
project(balance_msg)

# Load catkin and all dependencies required for this package
find_package(catkin REQUIRED COMPONENTS
  message_generation
)

########################
## Declare ROS message##
########################

# Generate messages in the 'msg' folder
add_message_files(
   FILES
   BalanceOdm.msg
   BalanceCmd.msg
 )

## Generate added messages with any dependencies listed here
generate_messages(
  DEPENDENCIES
)

###################################
## catkin specific configuration ##
###################################

catkin_package(
  CATKIN_DEPENDS message_runtime
)
