# Task_6

Launch Simulation World
_____________________________
In the previous SLAM section, TurtleBot3 World is used to creat a map. The same Gazebo environment will be used for Navigation.
CODE:
_______________
$ export TURTLEBOT3_MODEL=waffle
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch
________________________________
Screenshot:
_______________________

![6be86914-7d17-4e38-ba03-5bd6758c5b6d](https://user-images.githubusercontent.com/107879518/184558121-4bde7dc9-b537-49b3-96b7-4a1191c52d1d.png)
__________________________________
Run Navigation Node
__________
Open a new terminal from Remote PC with Ctrl + Alt + T and run the Navigation node.
_______________
CODE:
______________
$ export TURTLEBOT3_MODEL=waffle
$ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml
Screenshot:
_______________________

![aa8c9328-83d2-45e8-b23b-3b971a3120c1 (1)](https://user-images.githubusercontent.com/107879518/184558196-8e9498f5-ae30-4006-bfc8-f018e3be1064.png)
_______________________________________________
Estimate Initial Pose
_________________________
Initial Pose Estimation must be performed before running the Navigation as this process initializes the AMCL parameters that are critical in Navigation
TurtleBot3 has to be correctly located on the map with the LDS sensor data that neatly overlaps the displayed map.

Click the 2D Pose Estimate button in the RViz menu.
___________________________
Set Navigation Goal
______________________
Click the 2D Nav Goal button in the RViz menu. Click on the map to set the destination of the robot and drag the green arrow toward the direction where the robot will be facing.
Click on the map where the actual robot is located and drag the large green arrow toward the direction where the robot is facing.
________________________________
I uploaded a video (Task 6) showing the result.
