# ResearchTrack-I-First-assignment
A holonomic robot in a 2d space with a simple 2d simulator, Stage.
The exercise will be about a control of a holonomic robot in a 2d space. We want the robot to reach the target, and then ask for a new, random, target.

We will test the system with a simple 2d simulator, Stage by run the ((rosrun stage_ros stageros $(rospack find exercise1)/world/exercise.world))

The node controlling the robot will subscribe to the topic /odom and it will publish the velocity on the topic /cmd_vel.

Please follow these steps that I do:

1)A package, called exercise1 with dependencies: geometry_msgs, nav_msgs, roscpp.
