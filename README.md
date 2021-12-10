# openvslam_ros

This is a modified package to serve the purposes of [this project](https://github.com/csermac/mavros_px4_tests).
The main difference consists in defaulting to `ros` branch and having different topic names.

[OpenVSLAM](https://github.com/OpenVSLAM-Community/openvslam)'s ROS package.

## Subscribed topics

### monocular setup

- `camera/image_raw`

### stereo setup

- `camera/left/image_raw`
- `camera/right/image_raw`

### RGBD setup

- `camera/color/image_raw`
- `camera/depth/image_raw`

## Published topics

- `~/camera_pose`
- `~/pointcloud`
- `/tf`

## Parameters

- `odom_frame`
- `map_frame`
- `base_link`
- `camera_frame`
- `publish_tf`
- `publish_pointcloud`
- `transform_tolerance`
- `use_exact_time` (stereo, RGBD only)
