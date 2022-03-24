# Autonomous-Mobile-Robot 🤖 
![ROS](https://img.shields.io/badge/ros-%230A0FF9.svg?style=for-the-badge&logo=ros&logoColor=white)

## Introduction

In any supply chain, the warehouse is a main component in linking the chain partners and nowadays it acts as a competitive factor. Hence, it has become very necessary to manage warehouses effectively and allocate their resources efficiently. Warehouse Management Systems (WMSs) have been developed for monitoring, tracking, and controlling the warehouse operations, but with the increasing dynamicity of the market, traditional systems have become less efficient and unsuitable for today’s market requirements, that is why new technologies have started to emerge to be used for such applications. Internet of Things (IoT) is a promising technology that can be used in the context of Industry 4.0 


## Overview

autonomous mobile robot (AMR) is any robot that can understand and move through its environment without being overseen directly by an operator or on a fixed predetermined path. AMRs have an array of sophisticated sensors that enable them to understand and interpret their environment, which helps them to perform their task in the most efficient manner and path possible, navigating around fixed obstructions (building, racks, work stations, etc.) and variable obstructions (such as people, lift trucks, and debris).

![image](https://user-images.githubusercontent.com/102316688/159974956-98630c5c-9937-4bf9-a49e-25a6c428007e.png)

In a warehouse and distribution center environment, these sophisticated technologies are integrated with the warehouse’s control systems, which allow AMRs increased flexibility to create their own routes between locations within a warehouse or facility. The end result is a robot that is much better able to work with humans within the dynamic environment offered by most order fulfillment operations.
Autonomous mobile robots make processes and workflows more efficient and productive. This is typically achieved by performing non-value added tasks—such as transporting, picking up, and dropping off product—in order to free up laborers to perform other tasks that add value to the product/operation—like picking, checking, or packing an order.

## system overview

![image](https://user-images.githubusercontent.com/102316688/159981328-37300b8f-15d4-4502-af29-50e9741f6e7c.png)

## Dependencies 

- ROS Noetic
- Ubuntu 20.04 (LTS)


## `how to get started ? ;)`

`First`


after clone or download the repo 

```bash
cd home/agv_ws
```

```bash
catkin_make
``` 

### `start the environment & visualization` 
```bash
roslaunch agv_urdf gazebo.launch
```
### ` mapping (SLAM)`

```bash
roslaunch agv_slam auto_mapping.launch
```
![image](https://user-images.githubusercontent.com/102316688/159980946-8e634a66-8949-4d25-bf24-cf42d50a5f3a.png)


#### `After scanning the area `
```bash
rosrun map_server map_saver -f "name your map "
```
![image](https://user-images.githubusercontent.com/102316688/159979678-dafff9fb-300b-4ff1-971e-942bc15cb74e.png)

dont forget to change the map name in . yaml (configration files) in the file "agv_nav" its too important to make the next step work without errors 


### `Navigation `
```bash
roslaunch agv_nav navigation.launch
```
![image](https://user-images.githubusercontent.com/102316688/159981103-ce3ce2f4-b8b5-4894-a2d8-48093b99b26d.png)

## sources 
Books 

- ROS Robotics Projects: Build And Control Robots Powered By The Robot Operating System, Machine Learning, And Virtual Reality

- Mastering ROS for Robotics Programming: Best practices and troubleshooting solutions when working with ROS 

- Robot Operating System (ROS): The Complete Reference

Courses 

- ROS for Beginners: Basics, Motion, and OpenCV 

- ROS for Beginners II: Localization, Navigation and SLAM

## License
[MIT](https://choosealicense.com/licenses/mit/)
