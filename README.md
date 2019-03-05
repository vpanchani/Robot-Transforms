# Robot-Transforms


Project involved parsing thorugh URDF file and getting joint values, types and RPY values to generate a transform matrix.
It also establishes a link between parent and child node. Staring from wordlink, transforms are calculated to each joint which are then published and visulaized on rviz. 

To run the program - 
Use catkin_make to compile 
Run in different terminals - 
- roscore, 
- rosparam set robot_description --textfile kuka_lwr_arm.urdf
- rosrun robot_sim robot_sim_bringup
- rosrun robot_mover mover
- rosrun forward_kinematics solution.py 
- rosrun rviz rviz ( you will have to change link to word link and add robot model and tf)
