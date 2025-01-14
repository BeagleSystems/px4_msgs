# px4_msgs

[![GitHub license](https://img.shields.io/github/license/PX4/px4_msgs.svg)](https://github.com/PX4/px4_msg/blob/master/LICENSE) [![Build Status](https://travis-ci.org/PX4/px4_msgs.svg?branch=ros1)](https://travis-ci.org/PX4/px4_msgs)

This package contains the ROS(1) message definitions of the [PX4 Pro ecosystem](https://px4.io/). Building this package generates all the required interfaces to interface ROS nodes with the PX4 autopilot internals, which use the [uORB messaging API](https://dev.px4.io/en/middleware/uorb.html). Currently the messages of this package represent a dependency to [`px4_ros_com` package](https://github.com/PX4/px4_ros_com) `ros1` branch. The interface with PX4 is only possible using the [`ros1_bridge`](https://github.com/ros2/ros1_bridge) and `px4_ros_com`, which bridges the ROS topics with the ROS2 topics.

## uORB message definitions

The uORB message definitions, which represent the counter-part of these ROS messages found in this package, can be found on the [PX4 Firmware repository](https://github.com/PX4/Firmware).

## How are these messsage definitions generated?

The PX4 Firmware Jenkins-based CI/CD deploys new messages or modifications to the current definitions with each build of the master branch of the PX4 Firmware. A future improvement will also include tagging and releasing this repository according to the tags/releases of the PX4 Firmware, for a more tide coupling between the message definitions.

## Install, build and usage

Check [this](http://wiki.ros.org/ROS/Tutorials/CreatingMsgAndSrv) section of the ROS tutorials in order to understand how to create and build msg and srv files. Check the [RTPS/ROS2 Interface](https://dev.px4.io/en/middleware/micrortps.html) section on the PX4 Devguide for further details on how this integrates with the [`px4_ros_com` package](https://github.com/PX4/px4_ros_com).

## Bug tracking and feature requests

Use the [Issues](https://github.com/PX4/px4_msgs/issues) section to create a new issue. Report your issue or feature request [here](https://github.com/PX4/px4_msgs/issues/new).

## Questions and troubleshooting

Reach the PX4 development team on the `#messaging` PX4 Slack channel:
[![Slack](https://px4-slack.herokuapp.com/badge.svg)](http://slack.px4.io)
