StereoPi tutorial scripts
===========

Set of Disparity Map tutorial scripts for StereoPi board with CM3/3+ inside.

Was tested in the following environment:
* Raspbian Stretch (kernel 4.14.98-v7+)
* Python 3.5.3 
* OpenCV 3.4.4 (pre-compiled, 'pip' from Python Wheels)
* Picamera 1.13
* StereoVision lib 1.0.3 (https://github.com/erget/StereoVision)

Ready-to-use Raspbian Image:

[Download link 1 (Yandex Disk)](https://yadi.sk/d/KWYOwR3IIgTzAA)

[Download Link 2 (Google Drive)](https://drive.google.com/open?id=1sM37cT6dTlZHhSRIz4Z9oEJk_xbR7pLL)


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


