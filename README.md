# RoboND-Localization-Project
## Abstract
This project is the creation and testing of two robot simulations in a ROS (Robot Operating System) / Gazebo / RViz simulation environment. Both robots use Adaptive Monte Carlo Localization techniques combined with a navigation plugin to successfully navigate a maze to reach a predefined goal position. Please refer to [writeup](https://github.com/mgangster/RoboND-Localization-Project/blob/master/writeup.pdf) for explanation on code.

## Project Setup
First, downloads the repo to your Computer:
```sh
$ cd ~/robotics
$ git clone https://github.com/PatrickMockridge/UdacityWhereAmI.git
```
Then

```sh
$ cd ~/catkin_ws/
$ catkin_make
```

Now that you have a workspace, you can swap between Udacity Bot and the Rini2D2 by checking out the 'master' or 'new-robot' branches:
```sh
$ git checkout -b new-robot
$ bit checkout -b master
```
Build the project:
```sh
$ cd ~/catkin_ws
$ catkin_make
```
Source the terminal:
```
source ~/catkin_ws/devel/setup.bash
```

To run the program:
```sh
$ cd ~/catkin_ws
$ roslaunch udacity_bot udacity_world.launch
$ roslaunch udacity_bot amcl.launch
$ rosrun udacity_bot navigation_goal
```
