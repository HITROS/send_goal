下载此包，正常编译即可

想要在omtb里面使用此包，需要在导航launch文件里，把节点添加进去

```
<!-- 目标点位置 -->
 <include file="$(find simple_navigation_goals)/launch/send_goal.launch">
 </include>
```

可以自己去修改代码中的机器人的位置

```
goal.target_pose.pose.position.x = 1.0;
goal.target_pose.pose.position.y = 1.0;
```

添加一个脚本文件，可以实时查看机器人在世界坐标系中的位置，以此来计算导航精度

```
get_pose.py
```
