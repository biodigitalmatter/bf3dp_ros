# biomimic_fab_3dp_clay

Using ROS noetic

## Setup

### Install tooling

```bash
sudo apt-get update
sudo apt-get install python3-vcstool python-catkin-tools
```


### Setup catkin workspace
```bash
mkdir -p biomimic_fab_3dp_clay/src
cd biomimic_fab_3dp_clay/src
git clone https://github.com/biodigital_matter/biomimic_fab_3dp_clay

cd ..

vcs import src <src/biomimic_fab_3dp_clay/dependencies.rosinstall
rosdep update && rosdep install --from-paths src --ignore-src -r -y
catkin build 
```
