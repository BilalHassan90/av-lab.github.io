---
title: Khalifa University's Autonomous Shuttle (KUAS) Dataset
layout: page
permalink: /datasets/shuttle/
show_menu: false
---
<img src="/assets/KUAS_Dataset.png"/>
<h1 style="text-align:center"> <a href="https://drive.google.com/drive/folders/1pLg3zBLOQqoy38PMSnsyeirGmGAAIQVU"> Download here </a></h1>


The dataset includes around twenty minutes of unlabeled data (A set of 8 LiDARs, Monochrome Cameras, IMU, GPS) captured from an autonomous shuttle deployed in Khalifa University, SAN Campus, UAE. The vehicle is driving autonomously in a mixed traffic site inside the university campus, featuring different types of vehicles (sedans, SUVs, buses) as well as pedestrians on sidewalks, crossings, and on the road.
Data is provided in a rosbag format, with all transforms between sensors recorded.

Table I: Topics and datatypes

| Topic Name | # of Messages | Message Type |
| --- | --- | --- |
| /camera\_front\_acquisition\_details | 10532 | rds\_msgs/camera\_acquisition\_details |
| /camera\_front\_compressed | 10531 | sensor\_msgs/CompressedImage |
| /camera\_front\_mono | 10531 | sensor\_msgs/Image |
| /cameras/groups/all/sw\_trigger | 10653 | std\_msgs/Empty |
| /fusion\_pose | 106312 | geometry\_msgs/PoseWithCovarianceStampe |
| /gps/raw\_messages\_onchanged | 7 | std\_msgs/UInt8MultiArray |
| /gps/raw\_messages\_ontime | 10652 | std\_msgs/UInt8MultiArray |
| /gps\_bestpos | 5326 | rds\_msgs/msg\_novatel\_bestpos |
| /gps\_gpgst | 5326 | rds\_msgs/msg\_novatel\_gpgst |
| /gps\_origin | 1 | rds\_hal\_msgs/gps\_origin |
| /gps\_position | 5326 | rds\_msgs/localization\_gnss |
| /gps\_position\_horizontal | 5326 | rds\_msgs/localization\_gnss |
| /ldmrs\_pose | 26697 | rds\_msgs/localization\_lidar |
| /map\_ldmrs | 40 | nav\_msgs/OccupancyGrid |
| /measure\_odometry\_corrected | 52788 | rds\_msgs/odometry\_car |
| /mti\_node/imu/data | 106532 | sensor\_msgs/Imu |
| /mti\_node/imu/data\_corrected | 106437 | sensor\_msgs/Imu |
| /mti\_node/imu/data\_corrections | 2131 | sensor\_msgs/Imu |
| /mti\_node/imu/data\_horizontal | 106391 | sensor\_msgs/Imu |
| /rosout | 2 | rosgraph\_msgs/Log |
| /rosparam\_dump | 1 | std\_msgs/String |
| /scan\_ldmrs | 26801 | sensor\_msgs/PointCloud2 |
| /scan\_ldmrs\_front | 26627 | sensor\_msgs/PointCloud2 |
| /scan\_ldmrs\_front/raw | 26634 | rds\_msgs/RawScan |
| /scan\_ldmrs\_horizontal | 26793 | sensor\_msgs/PointCloud2 |
| /scan\_ldmrs\_loc | 26697 | sensor\_msgs/PointCloud2 |
| /scan\_ldmrs\_rear | 26625 | sensor\_msgs/PointCloud2 |
| /scan\_ldmrs\_rear/raw | 26634 | rds\_msgs/RawScan |
| /scan\_lms\_front\_left | 26613 | sensor\_msgs/PointCloud2 |
| /scan\_lms\_front\_left/raw | 26621 | rds\_msgs/RawScan |
| /scan\_lms\_front\_right | 26624 | sensor\_msgs/PointCloud2 |
| /scan\_lms\_front\_right/raw | 26634 | rds\_msgs/RawScan |
| /scan\_lms\_rear\_left | 26599 | sensor\_msgs/PointCloud2 |
| /scan\_lms\_rear\_left/raw | 26607 | rds\_msgs/RawScan |
| /scan\_lms\_rear\_right | 26627 | sensor\_msgs/PointCloud2 |
| /scan\_lms\_rear\_right/raw | 26634 | rds\_msgs/RawScan |
| /scan\_vlp16\_front | 10651 | sensor\_msgs/PointCloud2 |
| /scan\_vlp16\_front/raw | 21307 | rds\_msgs/RawScan |
| /scan\_vlp16\_rear | 10649 | sensor\_msgs/PointCloud2 |
| /scan\_vlp16\_rear/raw | 21306 | rds\_msgs/RawScan |
| /tf | 250463 | tf2\_msgs/TFMessage |
| /tf\_corrections | 1065 | geometry\_msgs/TransformStamped |
| /vehicle\_acceleration | 106436 | geometry\_msgs/AccelWithCovarianceStamped |
| /vehicle\_pose | 106309 | geometry\_msgs/PoseWithCovarianceStamped |
| /vehicle\_velocity | 106796 | geometry\_msgs/TwistWithCovarianceStamped |

