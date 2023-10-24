# 3001_Final_Project
Final Project code for RBE 3001.

Code is written in MATLAB and uses various available toolboxes to help (camera, color, etc.) the project.

Camera takes picture of objects to sort, and determines the colors of the balls on in its frame.
It orders the balls based on color priority arbitrarily assigned.
Lens corrections are performed, the centroid of each ball is found. 
Coordinates of the objects in the camera's frame are transformed to the robot's frame.
Inverse kinematics are performed to obtain the joint values needed to reach each ball.
For each ball in the queue, and for each joint, quintic trajctory is generated for smooth path to the ball.
Gripper closes and quintic trajectory is generated to reach the sorting location (already known for the color).
Gripper releases the ball in the sort location and the robot returns to home.
