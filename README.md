# SafeBot
### Object Tracking For Safety

Over the past few years, there has been extensive research on the topic of object tracking. The main aim of our projectis to develop a safety warning system by implementing multiple object tracking in videos using bounding boxes. It relys on **YOLO, a state-of-the-art object detection model**, to detect objects in the image frame and **the DeepSORT algorithm for tracking the detected objects**. Using an RGB-D dataset from **the Princeton Tracking Benchmark**, the transformed position coordinates of the tracked objects from the image frame(u, v, d) to the camera frame(x, y, z), the corresponding velocity vectors are calculated. These position and velocity vectors are then used to develop a **safety warning system which takes into consideration the distance and velocity at which the objects are approaching each other.**

There are many contexts in which this system is applicable – i) human-robot interactions e.g. collaborative robots, service robots ii) robot-robot interactions e.g. industrial robots iii) robot-object interactions e.g. obstacle avoidance in autonomous vehicles. Such environments are highly dynamic in nature and can easily lead to hazardous situations for the humans present. While most robots are equipped with IR sensors to perform tasks in their vicinity safely, it still leaves them with the disadvantage of being near-sighted. While humans can gauge danger instinctively, it is much harder to have a robot do the same. With such robots being deployed autonomously in human-interactive environments, a smart safety system which can issue warnings before possible collisions by simply taking in an RGB-D video stream would be very valuable.

### Object Tracking using YOLO and DeepSORT
<img src="https://github.com/malvika-shetty/SafeBot/blob/main/Results/Object%20Tracking/three_people_tracking_still.JPG" alt="Object Tracking" width="400"/>

### Safety Warning System
<img src="https://github.com/malvika-shetty/SafeBot/blob/main/Results/Safety%20Warning%20System/Frame_39.png" alt="Safety Warning System" width="500"/>
