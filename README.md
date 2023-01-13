# Eulerian Contour Path Planner

This planner generates a path that covers the object contours of a given area, which focuses on the particular objects and can be used for inspection, change monitoring, etc..

## Overview

This package provides an implementation of the path planner which is proposed in the paper .

This package acts as a global planner plugin to the Move Base package (http://wiki.ros.org/move_base).


## Installation

### Building from Source

#### Dependencies

- [Robot Operating System (ROS)](http://wiki.ros.org) (middleware for robotics),
- [Move Base Flex (MBF)](http://wiki.ros.org/move_base_flex) (move base flex node) used for system testing

#### Building

To build from source, clone the latest version from this repository into your workspace and compile the package using
```
cd catkin_workspace/src
git clone https://github.com/yongming-qin/eulerian_contour_path_planner.git
cd ../
catkin_make # or catkin build. depends on the build tool you are using
```

## Usage

Run a full navigation example using:

`roslaunch eulerian_contour_path_planner test_eulerian_contour_path_planner.launch`

Give an arbitrary 2D-goal in rviz to start the path planning algorithm. Since the planner covers the whole area, clicking the goal icon and pick any position will work.

Depends on:

[mobile_robot_simulator](https://github.com/mrath/mobile_robot_simulator.git) that integrates /cmd_vel into a base_link TF-frame and an odometry publisher

[tracking_pid](https://github.com/nobleo/tracking_pid/) Global path tracking controller


## Launch files

### test/eulerian_contour_path_planner/test_eulerian_contour_path_planner.launch




## Nodes





## References


## Bugs & Feature Requests

Please report bugs and request features using the [Issue Tracker](https://github.com/yongming-qin/eulerian_contour_path_planner/issues).

[ROS]: http://www.ros.org
[rviz]: http://wiki.ros.org/rviz
[MBF]: http://wiki.ros.org/move_base_flex

## Acknowledgments

While the algorithm is proposed by the authors, this package is written following the style of [Full Coverage Path Planner](https://github.com/nobleo/full_coverage_path_planner).
Secial thanks are given to the contributors of Full Coverage Path Planner.


## License

Apache 2.0

** Author(s): Yongming Qin **
** Maintainer: Yongming Qin, yq9vc@virginia.edu **
The Eulerian Coverage Path Planner package has been tested under [ROS] Noetic and Ubuntu 20.04.

