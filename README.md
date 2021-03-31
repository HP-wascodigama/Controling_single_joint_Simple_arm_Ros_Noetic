# Controling_single_joint_Simple_arm_Ros_Noetic
controlling single joint of simple_arm using user command and manipulate arm in ROS environment.
accessing camera data and processing for ferther control commands.

# steps
1. clone in /Home/catkin_ws/src.
2. $ cd ~/catkin_ws
3. $ catkin_make
4. $ source devel/setup.bash
5. $ rosdep install -i simple_arm
6. $ roslaunch simple_arm robot_spawn.launch
7. open new terminal and try
8. $ rosrun image_view image_view image:=/rgb_camera/image_raw
9. open new terminal and set value for joint agnle
10.$ rosservice call /arm_mover/safe_move "joint_1: 0.0 joint_2: 0.0"
