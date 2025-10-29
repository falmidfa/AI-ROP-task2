# AI-ROP-task2
- Installed **VirtualBox** 
- Created a new **Ubuntu** virtual machine inside VirtualBox
- Installed **Ros2 humble** on Ubuntu 
- Verifiede the installation and prepared the environment for running Ros2 commands
  
#Installed **Turtlesim** by using the following commads:**Terminal1**
- sudo apt update
- sudo apt install ros-humble-turtlesim
- source /opt/ros/humble/setup.bash
- ros2 pkg executables turtlesim

- To start turtlesim:
- source /opt/ros/humble/setup.bash
- ros2 run turtlesim turtlesim_node

- To run a new node:**Terminal2**
- source /opt/ros/humble/setup.bash
- ros2 run turtlesim turtle_teleop_key

- To add a new node or to change the size and width install **rqt**: **Terminal3**
- source /opt/ros/humble/setup.bash
- rqt 

- To run node2:
- source /opt/ros/humble/setup.bash
- ros2 run turtlesim turtle_teleop_key --ros-args -r turtle1/cmd_vel:=/turtle2/cmd_vel
