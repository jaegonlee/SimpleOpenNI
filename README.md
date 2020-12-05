# SimpleOpenNI
fix: compatible with processing 3

Tested: Mac OS X 10.11-10.15 / MBPR 15, iMac27 / Windows 10 / Kinect V1 / PrimeSense Sensor 

#### Install OpenNI2
https://github.com/OpenKinect/libfreenect/tree/master/OpenNI2-FreenectDriver

#### Install freenect
    $ brew install libfreenect
    $ git clone https://github.com/OpenKinect/libfreenect
    $ cd libfreenect
    $ mkdir build
    $ cd build
    $ cmake .. -DBUILD_OPENNI2_DRIVER=ON
    $ make

#### Copy library
    $ cp -L lib/OpenNI2-FreenectDriver/libFreenectDriver.dylib /example/openni2/Samples/Bin/OpenNI2/Drivers/

#### Run Demo
    $ cd /example/openni2/Samples/Bin/
    $ ./ClosestPointViewer

#### Build Sample
    $ cd /example/openni2
    $ source OpenNIDevEnvironment 
    $ cd /example/openni2/Samples/SimpleRead
    $ make

from:
https://blog.csdn.net/vincent2610/article/details/56282041
