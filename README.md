# water_simulation
Simulation of two wheeled differential robot.

The system is Ubuntu 16.04.

## To launch the robot in gazebo
$ roslaunch robot_description robot.launch

## To make map
### Gmapping: 
$ roslaunch nav_demo demo_1.launch

$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py

### Hector_slam:
$ roslaunch nav_demo hector_slam_demo.launch

$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py

### RRT:
(Notice: There are some problems with rrt. It always clashes the wall. Maybe the params of move_base.)

$ roslaunch rrt_exploration rrt_slam.launch

(Publish five points, four for the corners and the last for the robot point.)

## To use amcl especially:
$ roslaunch nav_demo demo_2.launch

## To navigate:
### move_base:
$ roslaunch nav_demo demo_3.launch
