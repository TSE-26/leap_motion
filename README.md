To run the panda_simulation with leap_motion, open 3 different terminals and follow these steps:

**Terminal 1:**
```
sudo LeapControlPanel
```
**Terminal 2:**
```
sudo leapd
```
To use the leap motion as the controller:

catkin_ws --> whatever you have called your workspace

**Terminal 1 Run the Panda simulation file: **
```
cd ~/catkin_ws
source devel/setup.bash
roslaunch panda_simulation simulation.launch
```
In the Motion Planning plugin of RViz, enable Allow External Comm. checkbox in the Planning tab

**Terminal 2 Run the Leap Motion python script:**
```
cd ~/catkin_ws
source devel/setup.bash
rosrun leap_motion LeapMove.py
```
**Terminal 3 Run the Leap Motion launch file:**
```
cd ~/catkin_ws
source devel/setup.bash
roslaunch leap_motion demo.launch
```
