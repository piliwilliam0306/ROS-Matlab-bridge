# ROS-Matlab-bridge

# Reocord Topics
## Record all topics.
  $ rosbag record -a
    
  ## Specify the maximum duration of the recorded bag file.
    $ rosbag record --duration=30 /topic
    
  ## Record to bag with name banana.bag.
    $ rosbag record -O banana.bag /topic


## Rosbag play
      $ rosbag play banana.bag
