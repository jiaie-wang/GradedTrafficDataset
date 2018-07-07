# Graded Traffic Dataset
We release a Graded Traffic Dataset which is organized by quantifying scenario complexity
## Motivation
<br>During the developing, testing and verification cycle of unmanned grounded vehicle (UGV) system, a large amount of traffic scenario data is utilized for performance evaluation. In recent years, to meet the practical demand of autonomous driving technology, especially for the research and development on environmental cognition and understanding algorithms, many traffic scene
datasets have been proposed, such as KITTI, RobotCar. These datasets are usually collected in traffic scenarios with dynamic changes in cognition complexity, including different types of roads, scene contents and scene characteristics. However, the lack of quantitative characterization of the scene complexity in these datasets could impede interpretable evaluation of UGV systems. On the other hand, in the unmanned off-line testing, we find that there is usually a negative correlation between the unmanned vehicle algorithm performance and scenario complexity. Traffic data with higher scenario complexity typically leads to worse performance of the environment cognition and understanding algorithm. If we use unorganized data to test and evaluate an environment-aware understanding algorithm for an unmanned system, the results are mostly indistinguishable: an algorithm with 0.84 overall accuracy may consistently perform worse than a competing algorithm with only 0.83 overall accuracy in common road scene scenarios. Therefore, the complexity of the scene data needs to be incorporated for reliable evaluation of UGV systems. Hence we propose a method in quantifying scenario complexity to rank massive scene data.\

## The Graded Traffic Dataset
This page contains our data recordings, sorted by scenario complexity. So far, we included only sequences, for which we either have 3D object labels. The dataset comprises the following information, captured and synchronized at 10 Hz:
><br>•	Processed (synced+rectified) color stereo sequences (0.5 Megapixels, stored in jpg format)\
><br>•	3D Velodyne point clouds (100k points per frame, stored as matlab file)\
><br>•	Calibration (Camera-to-Velodyne, stored as text file)\
><br>•	2D and 3D object tracklet labels (vehicle, stored as text file)\
><br>•	Semantic destriptor(stored as text file)

The data directory is shown as follows:
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/Image/fig2.png)
<br>Here,"synced+rectified" refers to the processed data where images have been rectified and undistorted and where the data frame numbers correspond across all sensor streams. Most people require only the "synced+rectified" version of the files.\
## Current capabilities for visual cognitive tasks
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/Image/fig1.jpg) 
<br>F1 scores of two intelligent vehicle contest participators A (shown in blue) and B (shown in orange), in the proposed Graded offline Evaluation(GOE) framework, with individual scores for roadway segments with three scenario complexities. 60%, 35% and 5% of the roadway segments are rated as simple, medium, and complex, respectively.\
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/records%20for%20FV%26PD.png)
<br>Records of GOE in lane detection evaluation. (a) Histograms of GOE results. (b)-(c) Cascaded tank model based visualization and comparison of Platform A and B, respectively.\
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/records%20for%20LD.png)
<br>Records of GOE in front vehicle and pedestrian detection. (a)Histograms of GOE results. (b)-(c) Cascaded tank model based visualization and comparison of Platform A and B, respectively.\
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/records%20for%20TS%26SD.png)
<br>Records of GOE in traffic sign & signal detection evaluation. (a)Histograms of GOE results. (b)-(c) Cascaded tank model based visualization and comparison of Platform A and B, respectively.\

## The introduction of Data segments 
### Simple data(1.34G)
<br>It Contains 5 data segments.\
<br>e.g.segment_001\
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/Gif/segment_001.gif)
<br>Length: 200 frames\
<br>Image resolution: 1920 x 620 pixels\
<br>Labels: 6 Cars\
### Medium data(630M)
<br>It Contains 4 data segments.\
<br>e.g.segment_007\
![image](https://github.com/jiaie-wang/GradedTrafficDataset/blob/master/Gif/segment_007.gif)
<br>Length: 32 frames\
<br>Image resolution: 1920 x 620 pixels\
<br>Labels: 12 Cars\
### Hard data(2.39G)
<br>It contains 13 data segments.\
<br>e.g.segment_015\
![image]()
<br>Length: 69 frames\
<br>Image resolution: 1920 x 620 pixels\
<br>Labels: 9 Cars\


>Note: We were not able to annotate all sequences and only provide those tracklet annotations that passed the 3rd human validation stage, ie, those that are of very high quality. For sequences for which tracklets are available, you will find the tracklets in the package. 

## Contact us
If you want to download this dataset, please contact us by E-mail: wangjiajie@stu.xjtu.edu.cn
