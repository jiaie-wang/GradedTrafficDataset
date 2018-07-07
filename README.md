# Graded Traffic Dataset
We release a Graded Traffic Dataset which is organized by quantifying scenario complexity
## Motivation

## The Graded Traffic Dataset
This page contains our data recordings, sorted by scenario complexity. So far, we included only sequences, for which we either have 3D object labels. The dataset comprises the following information, captured and synchronized at 10 Hz:
><br>•	Processed (synced+rectified) color stereo sequences (0.5 Megapixels, stored in jpg format)\
><br>•	3D Velodyne point clouds (100k points per frame, stored as matlab file)\
><br>•	Calibration (Camera-to-Velodyne, stored as text file)\
><br>•	2D and 3D object tracklet labels (vehicle, stored as text file)\
><br>•	Semantic destriptor(stored as text file)

The data directory is shown as follows:
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/Image/fig2.png)
Here,"synced+rectified" refers to the processed data where images have been rectified and undistorted and where the data frame numbers correspond across all sensor streams. Most people require only the "synced+rectified" version of the files.
## Current capabilities for visual cognitive tasks
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/Image/fig1.jpg) 
F1 scores of two intelligent vehicle contest participators A (shown in blue) and B (shown in orange), in the proposed Graded offline Evaluation(GOE) framework, with individual scores for roadway segments with three scenario complexities. 60%, 35% and 5% of the roadway segments are rated as simple, medium, and complex, respectively.
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/records%20for%20FV%26PD.png)
Records of GOE in lane detection evaluation. (a) Histograms of GOE results. (b)-(c) Cascaded tank model based visualization and comparison of Platform A and B, respectively.
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/records%20for%20LD.png)
Records of GOE in front vehicle and pedestrian detection. (a)Histograms of GOE results. (b)-(c) Cascaded tank model based visualization and comparison of Platform A and B, respectively.
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/records%20for%20TS%26SD.png)
Records of GOE in traffic sign & signal detection evaluation. (a)Histograms of GOE results. (b)-(c) Cascaded tank model based visualization and comparison of Platform A and B, respectively

## The introduction of Data segments 
### Simple data(1.34G)
It Contains 5 data segments.
e.g.segment_001
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/Gif/segment_001.gif)
Length: 200 frames
Image resolution: 1920 x 620 pixels
Labels: 6 Cars
### Medium data(630M)
It Contains 4 data segments.
e.g.segment_007
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/Gif/segment_007.gif)
Length: 32 frames
Image resolution: 1920 x 620 pixels
Labels: 12 Cars
### Hard data(2.39G)
It contains 13 data segments.
e.g.segment_015
![image]()
Length: 69 frames 
Image resolution: 1920 x 620 pixels
Labels: 9 Cars


>Note: We were not able to annotate all sequences and only provide those tracklet annotations that passed the 3rd human validation stage, ie, those that are of very high quality. For sequences for which tracklets are available, you will find the tracklets in the package. 

## Contact us
If you want to download this dataset, please contact us by E-mail: wangjiajie@stu.xjtu.edu.cn
