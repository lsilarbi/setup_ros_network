# setup_ros_network

## On the master comuter :

  - Open a terminal and tap ```hostname```

## On the remote computer :

  - Setup a fixed address direcly on linux, it must be on the same network than the one of the master computer
  - Open ```/etc/hosts``` file
  - Add the privious get hostname with the format ```ip_of_the_master_computer hostname```
  - Open .bashrc and add
```
export ROS_MASTER_URI=http://ip_of_the_master_computer:11311/
export ROS_IP=ip_of_this_computer
```

Test ```rostopic list``` then ```rostopic echo /a_topi```
