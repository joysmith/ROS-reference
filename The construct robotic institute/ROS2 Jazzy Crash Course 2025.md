- [youtube](https://www.youtube.com/watch?v=Se5pvRlTX8s)
- [ROS2 Jazzy Crash Course 2025](https://app.theconstruct.ai/rosjects/898950/)

### 1 Part

What is ROS2: ROS2 is an ecosystem/environment where several nodes/systems exchanges messages/data with each other to achieve some Behavioral

#### basic

- Package should always inside the ROS2 workspace "ros2_ws"
- rclpy ROS Client Library for Python (dependency): helps to create ros2 based python program
- ros2 run: allow to run only single python program **Where as** ros2 launch: allows to run _multiple_ python program
- ros2 launch file can be written in xml, yaml, python. python is the standard one
- setup.py: timestamp 31:00, explanation of os and install folder
- structure: simple_ros2.py(main program write) --> setup.py(generating executable from simple_ros2.py, linking to os)--> launch.py(configure package, executable)

#### ROS2 nodes

- nodes are just ros2 program written in python. so whenever we run ros2 program we create node
- What is ROS2: ROS2 is an ecosystem/environment where several nodes/systems exchanges messages/data with each other to achieve some Behavioral

<br>

### 2 Part: topic and multithreading

- What is topic: a topic is a channel where the information flows, and in that channel you can publish information to that channel or get information from that channel/pipe
-

<br>

### 3 Part: Rviz

- Rviz2: ros2 visualizer
- Rviz2 has model aka "visualizer" in technical term
- Gazibo is a simulation think like a real **robot** uses for experiment and rviz2 is using the **robot** data provided by gazebo simulation for visualizing
- Notics: my focus was on physic engine or simulation rather than robot in simulation. my focus should be on **robot** in simulation.

<br>

### 4 Part: Robot frames and transformer

-

<br>

### 5 Part: Robot frames and transformer

- There is no roscore in ROS2 like ROS1
-
