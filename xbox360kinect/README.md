# Xbox 360 Kinect on Ubuntu 20.04

This project space is used to document how I receieved live feed from the xbox 360 kinect programatically.


## Useful Links
[Open Kinect](https://github.com/OpenKinect/libfreenect)
[Setting up Kinect for programming in Linux (part1)](https://www.kdab.com/setting-up-kinect-for-programming-in-linux-part-1)
[Ros2 open source kinect driver](https://github.com/fadlio/kinect_ros2)

## quick hardware check
Check that the Xbox 360 kinect is being recognized by your device:
`lsusb`

The output should look something like this:
'''
Bus 001 Device 014: ID 045e:02ae Microsoft Corp. Xbox NUI Camera
Bus 001 Device 012: ID 045e:02b0 Microsoft Corp. Xbox NUI Motor
Bus 001 Device 013: ID 045e:02ad Microsoft Corp. Xbox NUI Audio
'''

## Open Source Libraries 
  * OpenKinect/libfreenect:
    - control Xbox 360 kinect motor, RGB and Depth images, LED, and audio

## install freebect
I initially began to read about a manual install but saw that there is official Ubuntu packaes to automate the installation for me!
`sudo apt-get install freenect`

personal note: in the midst of researching manual installation
I skipped this for testing.. may only be workaround to use sudo for using device resources
  * https://github.com/OpenKinect/libfreenect/tree/master/platform/linux/udev


