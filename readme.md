# smartcar_ws

## 目录结构
- racecar_description: 小车模型
- racecar_control: 控制运动, 包括电机控制、键盘遥杆控制
- racecar_slam: 建图、odom(坐标转换等)

## 启动

```shell 
# 启动建图
$ roslaunch racecar_slam make_map.launch
# ... 走一圈建图
$ rosrun map_server map_saver /xx/xx/map
```

```shell
# 建图结束, 用gazebo/rviz打开
$ roslaunch racecar_slam show_graph.launch
```