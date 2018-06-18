# ROS configuration and launch files for Neobotix MP-400

This package contains configuration and launch files for Neobotix MP-400.

![Neobotix MP-400](http://www.neobotix-roboter.de/fileadmin/files/produkte/Basisplattformen/MP-400/Roboter-MP-400-Hauptansicht.jpg)

The [MP-00](http://www.neobotix-robots.com/mecanum-robot-mp-400.html) is a small and effective mobile robot specialized for logistics.

# Contact information

For more information please visit our website at www.neobotix-robots.com. 
If you have any questions, just get in touch with us:
* General information: http://www.neobotix-robots.com/company-contact.html
* ROS related questions: ros@neobotix.de

# Installation

1. Create a catkin workspace (![tutorial](http://wiki.ros.org/catkin/Tutorials/create_a_workspace))

2. Download all packages listed under "Additionally required Neobotix-ROS-Packages" into your workspace

3. IMPORTANT! Delete all not used packages downloaded in step 2!

4. Install all packages listed under "Additionally required third party ROS-Packages"

5. Build your workspace


## Additionally required Neobotix-ROS-Packages:

Hardware connection: ![neo_relayboard_v2](https://github.com/neobotix/neo_relayboard_v2)

Kinematic: ![neo_mecanum_kinematics](https://github.com/neobotix/neo_kinematics_mecanum)

Laserscanner: ![cob_sick_s300](https://github.com/neobotix/neo_driver)

Scan-Merge: ![cob_scan_unifier](https://github.com/neobotix/neo_driver)

Teleoperation: ![neo_teleop](https://github.com/neobotix/neo_control)

Msgs: ![neo_msgs](https://github.com/neobotix/neo_msgs)

Srvs: ![neo_srvs](https://github.com/neobotix/neo_srvs)

## Additionally required third party ROS-Packages:

Joystick: [joy](http://wiki.ros.org/joy)

MoveBase: [move_base](http://wiki.ros.org/move_base) and [move_base_msgs](http://wiki.ros.org/move_base)

Teb Local Planner: [teb_local_planner](http://wiki.ros.org/teb_local_planner)

Eband Local Planner: [eband_local_planner](http://wiki.ros.org/eband_local_planner)

SLAM: [gmapping](http://wiki.ros.org/gmapping)

AMCL: [amcl](http://wiki.ros.org/amcl)

## Usage:

1. Edit the configuration of each ROS-Node to meet your needs 

2. Use the bringup.launch file for basic startup

3. Use the navigation.launch file for starting up MoveBase and SLAM or AMCL

4. Create your own .launch file

### ROSlaunch files:

Bringup: ![bringup.launch](https://github.com/neobotix/neo_mp_400/blob/indigo/launch/mp_400/bringup.launch)

Navigation with SLAM: ![navigation_basic_slam.launch](https://github.com/neobotix/neo_mp_400/blob/indigo/launch/mp_400/navigation_basic_slam.launch)

Navigation with AMCL: ![navigation_basic_amcl.launch](https://github.com/neobotix/neo_mp_400/blob/indigo/launch/mp_400/navigation_basic_amcl.launch)


### Configuration:

For each used ROS-Node there is a Folder in configs



