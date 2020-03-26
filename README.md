# Welcome to GO Chase it :robot:

In this project, I created two ROS packages inside my catkin_ws/src: the drive_bot and the ball_chaser. Here are the steps to design the robot, house it inside my world, and program it to chase white-colored balls: :ok_hand:

## Summary Tasks
* drive_bot:
- Create a my_robot ROS package to hold your robot, the white ball, and the world.
- Designed a differential drive robot with the Unified Robot Description Format. Add two sensors to your robot: a lidar and a camera. Add Gazebo plugins for your robot’s differential drive, lidar, and camera. 
- Placed the robot inside the world built in the Build My World project.
- Added a white-colored ball to Gazebo world and save a new copy of this world.
- The world.launch file should launch the world with the white-colored ball and your robot.
* ball_chaser: 
  - Created a ball_chaser ROS package to keep C++ nodes.
  - Write a drive_bot C++ node that will provide a ball_chaser/command_robot service to drive the robot by controlling its linear x and angular z velocities. The service should publish to the wheel joints and return back the requested velocities.
  - Write a process_image C++ node that reads robot’s camera image, analyzes it to determine the   - presence and position of a white ball. If a white ball exists in the image, your node should request a service via a client to drive the robot towards it.
  - The ball_chaser.launch should run both the drive_bot and the process_image nodes.
## Folder Files

![git](https://user-images.githubusercontent.com/51816415/77665582-c380a200-6f77-11ea-98b1-20f911f0f56f.JPG)

## Result 

![Animated GIF-downsized_large (1)](https://user-images.githubusercontent.com/51816415/77528045-280f0480-6e85-11ea-9770-7d6c2d0642b9.gif)

## Video

A short demo [videoclip](https://www.youtube.com/watch?v=7m-EOrbj6sM) (of a success case): can be found on my youtube Channel :boom:







