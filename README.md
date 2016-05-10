## ROSMASTER
      The ROS Master provides name registration and lookup to the rest of the Computation Graph. 
      Without the Master, nodes would not be able to find each other, exchange messages. 

## Node
      Nodes are processes that perform computation. 
      ROS is designed to be modular at a fine-grained scale; a robot control system usually comprises many nodes. 
      For example, one node controls a laser range-finder, one node controls the wheel motors, one node performs localization, one node performs path planning, and so on. 

## Messages
       Nodes communicate with each other by passing messages. 
       A message is simply a data structure, comprising typed fields. 
       Standard primitive types (integer, floating point, boolean, etc.) are supported, as are arrays of primitive types. Messages can include arbitrarily nested structures and arrays (much like C structs).

## Topic 
     Topics are buses used by nodes to transmit data. 
     A topic can have various subscribers.
     Each topic is strongly typed by the ROS message type used to publish it, and nodes can only receive messages from a matching type. 
     A node can subscribe to a topic only if it has the same message type.
     The topics in ROS can be transmitted using TCP/IP and UDP. The TCP/IP-based transport is known as TCPROS and uses the persistent TCP/IP connection. 
     
## rqt_plot
     $ rqt_plot feedback_wheel_angularVel/x feedback_wheel_angularVel/y 

## Record all topics.
     $ rosbag record -a

## Specify the maximum duration of the recorded bag file.
     $ rosbag record --duration=30 /topic
     $ rosbag record --duration=5m /topic

## Record to bag with name banana.bag.
     $ rosbag record -O banana.bag /topic  

## Rosbag play
      $ rosbag play banana.bag

## configuring ROS_MASTER_URI in matlab
     $ rosinit('http://will-UX32LN:11311')

## rqt_graph
     
## Reference

http://wiki.ros.org/rosbag
http://wiki.ros.org/rqt_plot
http://wiki.ros.org/rqt_graph
http://www.mathworks.com/help/robotics/examples/exchange-data-with-ros-publishers-and-subscribers.html
     
