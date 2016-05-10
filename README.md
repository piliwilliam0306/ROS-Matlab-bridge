
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
     $ rosinit('http://192.168.25.106:11311')
