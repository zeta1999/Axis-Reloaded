# Axis-Reloaded
This project uses 15 servo motors to articulate a robotic hand to rotate a platform, based on the popular project "Axis" made by Mark Setrakian. The hand will automatically correct the platform position if it starts to drift off center. A video of the original device in action can be seen [here](https://www.youtube.com/watch?v=EfQ6ygf7QE4) and our device [here](https://drive.google.com/open?id=1BuqYrJSDQ1Gmv87n5UrnKjRDvYjfAlRq).

The control algorithm plan trajectories for each of the 3-DOF fingers and calculates the inverse kinematic solutions to each discritized path. The Product of Exponentials forward kinematic solution is used, as well as a standard root solver for the inverse kinematics.  


# Hardware
A Raspberry Pi 3 Model B+ runs all the control algorithms. A Logitech C270 webcam provides visual feedback and the servo's used in the fingers are [Lynx Motion HT1's](http://www.lynxmotion.com/p-1127-lynxmotion-smart-servo-lss-motor-high-torque-ht1.aspx).


# Resources
* [Wiki](https://github.com/EricDavidWells/Axis-Reloaded/wiki) 
* [Lynx Motion Communication Protocol](https://www.robotshop.com/info/wiki/lynxmotion/view/lynxmotion-smart-servo/lss-communication-protocol/)


# Dependencies
* Python 3.6
* Scipy 1.3.2
* Matplotlib 3.1.1
* OpenCV 4.1.1.26
* Imultils 0.5.3
* [Lynxmotion Smart Servo Library](https://github.com/Lynxmotion/LSS_Library_Python)
