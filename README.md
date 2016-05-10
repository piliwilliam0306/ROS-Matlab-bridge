# ROS-Matlab-bridge

# Reocord Topics

## MCU firmware
     mega_base.ino is for mega board.
     vnh5019_left.ino is for the motor controller board which has "L" label.  
     vnh5019_right.ino is for the motor controller board which has "R" label.
     Please select Arduino Pro Mini when uploading codes for the motor controller boards.
     Current sense in A0: 5V / 1024 ADC counts / 144 mV per A = 34 mA per count


## Record all topics.

  $ rosbag record -a
  
## Specify the maximum duration of the recorded bag file.

  $ rosbag record --duration=30 /topic
    
## Record to bag with name banana.bag.

  $ rosbag record -O banana.bag /topic

## Rosbag play
      $ rosbag play banana.bag
