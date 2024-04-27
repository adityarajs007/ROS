# ROS
ROS | Robotics

The project utilizes ROS to simulate the palletizing action. It achieves this task using image processing libraries and robot control.

Libraries used for this project are majorly rospy, opencv

# File Description

1. controller.py : Controls the Robot simulation and paramters like the gripping force, the speed of the arm movement and similar parameters.
2. object_detection.py: It does the job to detect hte colored obstacles on the workbench and defines the bounding boxes on them as seen in the video. This code also perform camera calibration and generates simulation world coordinates from the images of t colored blocks. This imulation world coordinates, help the robot to actually reach and pick up the block.
3. pick_and_place_state_machine.py: This file controls the stae of the robot like "Home" and the "Selecting this colored block " states for keeping track of the sgtgate of the robotic simulation arm and help it to achieve its task of palletizing all the objects on the workbench.
