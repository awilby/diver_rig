# diver_rig

## Installation

Install ROS package dependencies from Ubuntu repositories:

`sudo apt-get install ros-kinetic-robot-state-publisher ros-kinetic-robot-localization`

Clone this repository, including submodules:

`git clone --recurse-submodules https://github.com/awilby/diver_rig.git`

Build everything from catkin workspace:

```cd <your_catkin_workspace>
catkin build
```


## Launch

Two top-level launch files are included for launching all systems on the diver rig. The difference between these two is the position of the IMU (when testing in the lab, the IMU is put on the chassis, but when in the field it is in the underwater housing with the Fitlet and batteries). Use `roslaunch diver_rig_air_config.launch` for testing in the lab and `roslaunch diver_rig.launch` for underwater usage.
