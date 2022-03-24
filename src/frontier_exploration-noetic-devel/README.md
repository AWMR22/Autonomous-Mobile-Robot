# frontier_exploration

Thread safe frontier exploration package based on fast and efficient Wavefront Frontier Detection.

## Resolving dependencies

Use `rosdep` to resolve ROS dependencies

## References

```
@misc{topiwala2018frontier,
      title={Frontier Based Exploration for Autonomous Robot}, 
      author={Anirudh Topiwala and Pranav Inani and Abhishek Kathpal},
      year={2018},
      eprint={1806.03581},
      archivePrefix={arXiv},
      primaryClass={cs.RO}
}
```

## Demo using Turtlebot3

- **Shell #1** : Gazebo

```bash
roslaunch turtlebot3_gazebo turtlebot3_world.launch
```

- **Shell #2** : SLAM + RViz

```bash
roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping
```

- **Shell #3** : move_base

```bash
roslaunch turtlebot3_navigation move_base.launch 
```

- **Shell #4** : Frontier exploration

```bash
roslaunch frontier_exploration explore_costmap.launch
```