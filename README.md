# NeuronBot2 Multibot
## Installzation
```bash
source /opt/ros/melodic/setup.bash
mkdir -p ~/multibot_ws/src/neuronbot2
cd ~/multibot_ws/src/neuronbot2
git clone https://github.com/skylerpan/neuronbot2_multibot
cd neuronbot2_multibot
vcs import < neuronbot2_multibot.repos
mv neuronbot2/* .. && rm neuronbot2 -rf
cd ~/multibot_ws
rosdep install --from-path src --ignore-src -r -y
catkin_make
```
## Setup ROS1 environment
```bash
source /opt/ros/melodic/setup.bash
source ~/multibot_ws/devel/setup.bash
```
## Run NeuronBot2 Multibot
```bash
roslaunch neuronbot2_multibot start.launch
```