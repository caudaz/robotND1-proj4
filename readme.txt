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
(RoboND) a1@p3510:~/robotND1-proj4/code$ pwd
/home/a1/robotND1-proj4/code
(RoboND) a1@p3510:~/robotND1-proj4/code$ python follower.py model_weights

