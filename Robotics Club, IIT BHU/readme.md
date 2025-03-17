- ROS is not an OS but it behave like an OS, for instance think of linux kernel it integrate all hardware(keyboard, mouse, pendrive, display, sound) level driver and provide an abstraction layer.

- package: a package provide all the feature of a specific component for instance ultrasonic sensor. feature could be: get the distance, is there any obstacle.
- message: a type(int, float, bool) of data shared between nodes
- topic: a robot data from a specific sensor(ultrasonic)
- publisher: data is always publish on topic, and a publisher publish sensor data
- subscriber: subscribe to a topic
-

<img src="../assets/images/ROS WORKSHOP 1/1.png" width="800">

<img src="../assets/images/ROS WORKSHOP 1/2.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/3.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/4.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/5.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/6.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/7.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/8.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/9.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/10.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/11.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/12.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/13.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/14.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/15.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/16.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/17.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/18.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/19.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/20.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/21.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/22.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/23.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/24.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/25.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/26.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/27.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/28.png" width="700">

<img src="../assets/images/ROS WORKSHOP 1/29.png" width="700">

```sh
# 1 Terminal: mater node running on raspberry
roscore

# 2 Terminal: rosrun is cmd,turtlesim is a folder, then press tab to get different nodes
# create turtlebot
rosrun turtlesim
rosrun turtlesim turtlesim_node

# 3 Terminal: list out running nodes
rosnode list

# 3 Terminal: rosrun is cmd,turtlesim is a folder, then press tab to get different nodes
rosrun turtlesim
rosrun turtlesim turtle_teleop_key

# 4 list out all topics
rostopic list
# list out all topics with subscriber and publisher
rostopic list -v

# type cmd and press TAB
rostopic
# type cmd and press TAB
rostopic pub /
# type cmd and edit x,y,z linear & angular
rostopic pub /turtle1/cmd_vel geometry_msgs/Twist

# run for specific time
rostopic pub --once /turtle1/cmd_vel geometry_msgs/Twist

# this wont show anything because we haven't got any subscriber
rostopic pub /turtle1/pose turtlesim/Pose

rosservice
# run cmd and press TAB
rosservice call /
# How to create a new turtlebot (fill information)
rosservice call /spawn
# to get all running topics
rostopiclist

```

#### Where to get all ros2 binary file in system

my computer--> opt -->ros -->melodic -->lib
