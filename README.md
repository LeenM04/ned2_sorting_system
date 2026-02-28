# Automated Sorting & Logistics System using Niryo Ned2 🤖

This project was developed as part of the **Intelligent Robotics** course at the **University of Jordan** It demonstrates an end-to-end industrial automation pipeline integrating robotic manipulation, computer vision, and sensor-based synchronization.

## 🔄 System Workflow
The system automates a complex sorting task through the following synchronized steps:

1.  **Object Retrieval**: The **Niryo Ned2** (6-axis collaborative arm) picks colored cubes from a side storage stand.
2.  **Conveyor Transport**: Objects are placed onto a conveyor belt which moves them toward the inspection zone.
3.  **Smart Stop (IR Trigger)**: An **Infrared (IR) sensor** detects the object’s arrival, signaling the conveyor to stop at the precise location for visual analysis.
4.  **Computer Vision Pipeline**:
    * The **Niryo Vision Camera** captures a frame of the workspace.
    * **Pre-processing**: Gaussian Blur and Canny Edge Detection are applied to reduce noise and find object contours.
    * **Classification**: Color masking identifies the object as **Red**, **Blue**, or **Green**.
5.  **Targeted Sorting**: Based on the identified color, the robot picks the cube and places it in front of the corresponding "Car" drop-off zone (or the trash for unknown items).



## 🛠️ Technical Stack
* **Robot**: Niryo Ned2 Collaborative Arm.
* **Software**: Python-based control script integrated with ROS2.
* **Vision**: OpenCV-based processing for contour detection and color masking.
* **Hardware**: Conveyor Belt, IR Sensors, and Custom 3D-printed Gripper.

## 👥 Project Team 
This project was a collaborative effort by Team 9:
* Asya Samer, Dana Abu Al Ruz, Ethar Al Salameh, Layla Lahham, Jana Saleh Godieh, **Leen Al Masarweh**, Rahaf Elayyan, Ksandra Haddad, Sewar AlRihani.
* **Supervised by**: Dr Musa Al-Yaman.


*Created for the University of Jordan - King Abdullah II School for IT.*
