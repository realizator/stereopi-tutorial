StereoPi tutorial scripts
===========

Set of Disparity Map tutorial scripts for StereoPi board with CM3/3+ inside.

Was tested in the following environment:
* Raspbian Stretch (kernel 4.14.98-v7+)
* Python 3.5.3 
* OpenCV 3.4.4 (pre-compiled, 'pip' from Python Wheels)
* Picamera 1.13
* StereoVision lib 1.0.3 (https://github.com/erget/StereoVision)


Brief scripts description:

<b>1_test.py</b> - starts camera preview, save captured image if 'Q' button pressed. 
align.
<br>

<b>2_chess_cycle.py</b> - takes a series of photos for stereopair calibration, shows count
down timer. You need a printed chessboard with 9x6 parameters (file "pattern.png" included).<br>
<br>

<b>3_pairs_cut.py</b> - just cuts all captured photos to left and right images.<br>
<br>

<b>4_calibration.py</b> - calibrate StereoPi cameas setup using pairs from script 4.<br>
<br>


<b>5_dm_tune.py</b> - script for fine tune of disparity map settings.<br>
<br>

<b>6_dm_video.py</b> - builds disparity map in real time.<br>
<br>


