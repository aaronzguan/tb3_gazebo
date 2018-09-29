# tb3_gazebo
 Gazebo simulation with Turtlebot 3 for recognizing AR Tags
 
 ![demo](https://github.com/aaronzguan/tb3_gazebo/blob/master/images/arena.png)
 
 ## Requirements
* **ROS Kinetic + Gazebo**
* tb3_description (URDF file of turtlebot 3)
* _Joy Package (optional)_
* _rqt (optional)_

## Installation

If you have an active ROS workspace, clone or download the repository into the src directory of your workspace:
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/aaronzguan/tb3_gazebo.git
```

Next install missing dependencies using rosdep install:
```
$ cd ~/catkin_ws
$ rosdep install --from-paths src --ignore-src --rosdistro=kinetic -y
```

Build:
```
$ cd ~/catkin_ws
$ catkin_make
```

If you haven’t already, the following line can be added to your .bashrc to auto-source all new terminals:
```
source ~/catkin_ws/devel/setup.bash
```

## Usage

```
$ roslaunch tb3_gazebo tb3_gazebo.launch
```

In a new terminal tab you can launch rqt:

```
$ rqt
```
Then in the Plugins menu, select "Robot Tools", and "Robot Steering".
