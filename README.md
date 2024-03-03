# task3-adding-imu
In this task we will add an imu to the mobile manipulator along with an imu gazebo plugin 
Gazebo Plugins are an extremely important and useful component of the software system.
We use these to add sensors and receive values from the virtual rover which can be later used for multiple tasks.
For more information refer to:
https://classic.gazebosim.org/tutorials?tut=ros_gzplugins

In this task we will add an IMU sensor to our mobile manipulator robot. What is an imu sensor? An Inertial Measurement Unit (IMU) is a device that can measure and report specific gravity and angular rate of an object to which it is attached. An IMU typically consists of: Gyroscopes: providing a measure angular rate. Accelerometers: providing a measure specific force/acceleration. To read more on IMU https://www.seeedstudio.com/blog/2020/01/17/what-is-imu-sensor-overview-with-arduino-usage-guide/

With a gazebo plugin we can simulate this imu in a simulation ... So how do we do it?

STEP1: Recollect how we added a lidar in the mobile manipulator. Adding the imu will also consists of the same method. 
        a) Learn how to make a link for the imu 
        b) Dimensions of the link should be same as that you of the lidar 
        c) Create a joint that connects the imu link to the base_link
        d) The joint should be of the type ```fixed``` and it should be exactly 10 cm above the lidar. 
        
STEP 2: Now that you have added the link ... add a imu gazebo plugin 
        ( take help of youtube videos and articles online)

Your task is to use the gazebo plugins to add an IMU sensor to the rover by changing the urdf file and receive the imu data.
The name of the topic should be /imu.
Publish the data by running ```rostopic echo /imu``` in the terminal

STEP 3: Submit the Screenshot of the imu data being published and the urdf file.
        
