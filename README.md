# ResearchTrack-I-First-assignment
A holonomic robot in a 2d space with a simple 2d simulator, Stage.
The exercise will be about a control of a holonomic robot in a 2d space. We want the robot to reach the target, and then ask for a new, random, target.

We will test the system with a simple 2d simulator, Stage by run the ((rosrun stage_ros stageros $(rospack find exercise1)/world/exercise.world))

The node controlling the robot will subscribe to the topic /odom and it will publish the velocity on the topic /cmd_vel.

Please follow these steps that I do:

1)A package, called exercise1 with dependencies: geometry_msgs, nav_msgs, roscpp.

2)Put the source code exercise.cpp in the src directory of the new package.

3)Put the files exercise.world and uoa_robotics_lab.png in the world folder of the new package.

4)Create another package, with dependencies: roscpp, std_msgs, message_generation.

5)Put the source code PositionServer.cpp in the src directory of the new package.

6)create a service message (using this second package) with an empty request, and two floats (x and y) as response.

7)modify exercise1.cpp so as to reach the target with the robot. When the target is reached, the node should require the service to send a new target position.
