# ros1_pepper_navreqs
Contains packages required to cross compile the navigation stack for pepper for ros1.


When cross compiling the navigation stack, add this repo to the repos list (pepper_ros1.repos):  
```
ros1_pepper_navreqs:
    type: git
    url: https://github.com/simwijs/ros1_pepper_navreqs.git
    version: master
    
```
  
  NOTE: There are several other dependencies, but because of conflicts of the packages tf2_sensor_msgs and visualization_msgs, this repository was created to avoid those conflicts. This means that you do not need to add tf2_sensor_msgs and visualization_msgs at all if you instead add this repository to your repos list.
