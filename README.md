# ROS3_navvis
## **Package description**
  - This package contains the code implementation for Lab2, which includes the basic modeling for a classic Navvis robot.

## **Dependency**
To view this model, these listed dependencies should be satisfied:
  - ROS (Neotic)
  - ROS velodyne-description
  - gazebo (plugins)

## ** Run**
There are several different ways to view this model,
Before viewing the model, make sure to:
Download the package into

`catkin_ws/src/`

Build the package

`catkin_make`

Then source:

`source catkin_ws/devel/setup.bash`

1. Start up the RVIZ to view the URDF version of the model (Use Joint_state_publisher gui by default)
`roslaunch navvis_description navvis_launch.launch`

2. Start up the RVIZ to view the XACRO version of the model
`roslaunch navvis_description navvis_launch.launch use_xacro:=true`

3. Start up the RVIZ to view the model WITHOUT Joint_state_publisher:
`roslaunch navvis_description navvis_launch.launch use_gui:=false` 

Note: options to launch this model:
- `use_xacro:= [true/false]` - true: use xacro file / false: use urdf file
- `use_gui:= [true/false]` - true(default): use the Joint State Processor Gui / false: donot use
