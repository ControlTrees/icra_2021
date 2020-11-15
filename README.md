# icra_2021

This repo contains the code for 2 examples of the ICRA 2021 submission.

[Accompanying video](https://youtu.be/Ju5hv2gIlxw)

## Installation

ros

gazebo

install models

clone, with submodules

build rai

catkin_make

## Execute tests
Open a terminal in the folder corresponding to the `control_tree_car` package in `build` folder of the catkin workspace.
This is typically `${CATKIN_WORKSPACE}/build/icra_2021/control_tree_car` where `CATKIN_WORKSPACE` is the root of the catkin workspace.

```bash
ctest .
```

## Launch examples

### Pedestrian example
Open two terminals in the catkin workspace.

In the first terminal, type the following command, it will launch the planner and the visualization RViz.
```bash
roslaunch control_tree_car pedestrian.launch
```

In the second terminal, type the following command, it will launch the simulator.
```bash
gzserver src/icra_2021/lgp_car_gazebo_plugin/world/pedestrian_4.world
```

### Obstacle avoidance example
Open two terminals in the catkin workspace.

In the first terminal, type the following command, it will launch the planner and the visualization RViz.
```bash
roslaunch control_tree_car obstacle_avoidance.launch
```

In the second terminal, type the following command, it will launch the simulator.
```bash
gzserver src/icra_2021/lgp_car_gazebo_plugin/world/obstacle_avoidance_2.world
```
