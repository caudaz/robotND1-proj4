create a link to:
Segmentation-Lab
controls lab1
conrtrols lab2
theory

concepts learned:
-Controls
-FCN
-1d convolutions
-batch normalization
-etc
-keras

-how to take data - what to look for

~/robotND1-proj4/code$ python preprocess_ims.py

The folders data/train/images/, data/train/masks/, data/validation/images/, and data/validation/masks/ should exist and contain the appropriate data
~/robotND1-proj4/data$ cp -r processed_sim_data/* .


USING WEIGHTS to FOLLOW ME
1
Then start simulatro "spawn people" mode, click "follow me" button

2
(RoboND) :~/robotND1-proj4/code$ pwd
/home/a1/robotND1-proj4/code
(RoboND) :~/robotND1-proj4/code$ python follower.py model_weights



NUMPU FIX to PROCESS IMAGES

Basically, the latest numpy version is 1.14.2, but you want to go back to 1.13.1 -- this fixed the problem for me.

If you are using Anaconda, go to your Anaconda terminal and type:

pip install numpy==1.13.1

This error would not create the correct number of masks per JPEG created

============================

(RoboND) :/mnt/c/UDACITY-robotics4/robotND1-proj4/code# python preprocess_ims.py
  File "/root/miniconda3/envs/RoboND/lib/python3.5/site-packages/scipy/misc/pilutil.py", line 97, in bytescale
    cscale = cmax - cmin
TypeError: numpy boolean subtract, the `-` operator, is deprecated, use the bitwise_xor, the `^` operator, or the logical_xor function instead.

(RoboND) :/mnt/c/UDACITY-robotics4/robotND1-proj4/code# python
>>> import numpy
>>> numpy.version.version
'1.14.5'

(RoboND) :/mnt/c/UDACITY-robotics4/robotND1-proj4/code# pip install numpy==1.13.1
Successfully uninstalled numpy-1.14.5
Successfully installed numpy-1.13.1

============================

(RoboND) :/mnt/c/UDACITY-robotics4/robotND1-proj4/code# python preprocess_ims.py

NO ERRORS!
