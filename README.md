author: le.gentil.cedric@gmail.com

## IN2LAAMA datasets

This repository provides lidar-inertial datasets collected with a Velodyne VLP-16 lidar and a Xsens MTi-3 IMU.
The lidar data is collected with the [snark driver](https://github.com/acfr/snark).
The IMU data is collected with rosbags and the ROS [xsens\_driver](http://wiki.ros.org/xsens_driver).
The calib.csv file provide the extrinsic calibration between the sensors:

- Format : r\_c1,r\_c2,r\_c3,p\_c1,p\_c2,p\_c3
- Rotation (r\_c) in euler angles in radians with the ZYX convention (mathlab's one)
- Translation (p\_c)
- A lidar point is reprojected in imu frame via x\_i = R\_c * x\_l + p\_c

## Reference

Please cite the following paper if this dataset is use in academic work

```bibtex
@ARTICLE{9194310,
  author={Le Gentil, Cedric and Vidal-Calleja, Teresa and Huang, Shoudong},
  journal={IEEE Transactions on Robotics}, 
  title={IN2LAAMA: Inertial Lidar Localization Autocalibration and Mapping}, 
  year={2021},
  volume={37},
  number={1},
  pages={275-290},
  doi={10.1109/TRO.2020.3018641}}
```
[IEEE](https://ieeexplore.ieee.org/document/9194310)

[Arxiv](https://arxiv.org/abs/1905.09517)


## Copyright

Datasets on this page are copyright by us and published under the [Creative Commons Attribution-NonCommercial-ShareAlike 3.0 License](https://creativecommons.org/licenses/by-nc-sa/3.0/). This means that you must attribute the work in the manner specified by the authors, you may not use this work for commercial purposes and if you alter, transform, or build upon this work, you may distribute the resulting work only under the same license.

