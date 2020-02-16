StereoPi tutorial scripts
===========

Set of Disparity Map tutorial scripts for StereoPi board with CM3/3+ inside.

Brief tutorial: [article in our Blog](https://stereopi.com/blog/opencv-and-depth-map-stereopi-tutorial)

Was tested in the following environment:
* Raspbian Stretch (kernel 4.14.98-v7+)
* Python 3.5.3 
* OpenCV 3.4.4 (pre-compiled, 'pip' from Python Wheels)
* Picamera 1.13
* StereoVision lib 1.0.3 (https://github.com/erget/StereoVision)

### Critical notice!
In the latest Raspbian kernels stereoscopic support has been occasionally broken by implementing new AWB algorithm. You can read some details [here](https://github.com/raspberrypi/firmware/issues/1253). Our Raspbian image provided has no such a problem, but you can get it after 'apt-get upgrade' or 'rpi-update'.

Current solution: after boot run once this command before accessing your cameras:
```
sudo vcdbg set awb_mode 0
```
This will turn AWB algo to the previous mode, and stereo works again untill next reboot. So run this command after reboot, or add it to your autorun script. 



Ready-to-use Raspbian Image:

[Download link 1 (Yandex Disk)](https://yadi.sk/d/KWYOwR3IIgTzAA)

[Download Link 2 (Google Drive)](https://drive.google.com/open?id=1sM37cT6dTlZHhSRIz4Z9oEJk_xbR7pLL)

## Important notice for Linux users.
I'd like to thank tuxlifan user for this information!

WARNING for Linux users: please do NOT use unzip to extract the zip file but use "7z e stereopi-opencv-20190405.zip" instead.

Checksum for stereopi-opencv-20190405.zip file is:
sha256: 6c7a5714db03aae07aeb009483f3fcd0fa43356280da071fdc3bad31dfe6f0c4
md5: fa82c9b997f6797c8445602b933b6ae4)

md5sum using unzip (and getting an error message about "Bad CRC"): 3ce7a63479ffa65fc923297d1fa01792
md5sum using 7z:
8dbe549e3a467a583a961bad85e45ca1

## Brief scripts description:

Press 'Q' key in any script for exit, as we added key stroke processing. Do not kill it by Ctrl+C :) 

<b>1_test.py</b> - starts camera preview, save captured image if 'Q' button pressed.

Video: https://www.youtube.com/watch?v=wllLrNUw3SE
<br>

<b>2_chess_cycle.py</b> - takes a series of photos for stereopair calibration, shows countdown 
timer. You need a printed chessboard with 9x6 parameters (file "pattern.png" included).

Video: https://youtu.be/1XCAlU3k-xs

<br>

<b>3_pairs_cut.py</b> - just cuts all captured photos to left and right images.<br>

Video: https://youtu.be/95DWmPECbDc

<br>

<b>4_calibration.py</b> - calibrate StereoPi cameas setup using pairs from script 4.

Video: https://youtu.be/vtPhu23tKGo

<br>


<b>5_dm_tune.py</b> - script for fine tune of disparity map settings.<br>

Video: https://youtu.be/Z4j3NrMyeGE

<br>

<b>6_dm_video.py</b> - builds disparity map in real time.<br>

Video: https://youtu.be/f29arVstfZA

<br>


