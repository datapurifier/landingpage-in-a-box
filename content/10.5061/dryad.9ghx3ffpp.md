---
title: "mRI: multi-modal 3d human pose estimation dataset using mmwave, rgb-d, and inertial sensors"
doi: 10.5061/dryad.9ghx3ffpp
referralUrl: https://datadryad.org/stash/dataset/doi:10.5061/dryad.9ghx3ffpp
categories:
- Dataset
tags:
- FOS: Computer and information sciences
- rehabilitation
- human pose estimation
- mmWave
- healthcare
publishers:
- Dryad
author:
- An, Sizhe
affiliations:
- University of Wisconsin-Madison
funders:
- National Science Foundation
---

# Abstract
The ability to estimate 3D human body pose and movement, also known as human pose estimation~(HPE), enables many applications for home-based health monitoring, such as remote rehabilitation training. Several possible solutions have emerged using sensors ranging from RGB cameras, depth sensors, millimeter-Wave (mmWave) radars, and wearable inertial sensors. Despite previous efforts on datasets and benchmarks for HPE, few datasets exploit multiple modalities and focus on home-based health monitoring. To bridge this gap, we present mRI, a multi-modal 3D human pose estimation dataset with mmWave, RGB-D, and Inertial Sensors. Our dataset consists of over 5 million frames from 20 subjects performing rehabilitation exercises and supports the benchmarks of HPE and action detection. We perform extensive experiments using our dataset and delineate the strength of each modality. We hope that the release of mRI can catalyze the research in pose estimation, multi-modal learning, and action understanding, and more importantly, facilitate the applications of home-based health monitoring.

## TechnicalInfo
mRI: multi-modal 3d human pose estimation dataset using mmwave, rgb-d, and inertial sensors [Access this dataset on Dryad](https://doi.org/10.5061/dryad.9ghx3ffpp) Data storage for NeurIPS 2022 paper [mRI: multi-modal 3d human pose estimation dataset using mmwave, rgb-d, and inertial sensors](https://proceedings.neurips.cc/paper_files/paper/2022/hash/af9c9c6d2da701da5a0acf91ec217815-Abstract-Datasets_and_Benchmarks.html) Update 11/27/2023: We fixed the bug in the videos zip file. ## Data and file structure There are two main sections of the data. ### RGB video data: blurred\_videos.zip There are 40 videos for 20 subjects (left and right each). ### Other raw data, features, and model: dataset\_release.zip The folder structure should be like this: ``` ${ROOT} |-- raw_data | |-- imu | |-- eaf_file | |-- radar | |-- unixtime | |-- videolabels |-- aligned_data | |-- imu | |-- radar | |-- pose_labels |-- features | |-- imu | |-- radar |-- model | |-- imu | | |-- results | | |-- *.pkl | |-- mmWave | | |-- results | | |-- *.pkl ``` ***Tabular header explanation*** * csv raw data under features/imu/subject*: * address: IMU ID * axg, ayg, azg: Acceleration in three axis * AngleXdeg, AngleYdeg, AngleZdeg: Euler angle * q0,q1,q2,q3: Quaternion (we only used these to obtain the .pt file) * csv radar raw data under rawdata/radar: * Frame #: Index of frame * \# Obj: How many points detected in this frame * X, Y, Z: 3D coordinates of points * Doppler: Doppler velocity * Intensity: Reflected power intensity * Time: Wall timestamp ***Load cpl file*** The .cpl file is essentially pickle file, to read them, use: ``` import pickle file = pickle.load(open('.../file_path/XXX.cpl', 'rb')) ``` ***raw_data*** folder contains all raw_data before synchronization. It includes imu raw data, radar raw data, eaf annotations, unix timestamp from camera, and videolabels generated from the eaf file. ***aligned_data*** folder contains all data after temporal alignment. It includes imu data, radar data, and the pose_labels. pose_labels for each subject contain following information: * '2d_l_avail_frames': available frames for 2d human detection, left camera * '2d_r_avail_frames': available frames for 2d human detection, right camera * 'camera_matrix': camera parameters * 'gt_avail_frames': available frames for 3d human joints ground truth * 'imu_avail_frames': available frames for imu-estimated keypoints * 'imu_est_kps': imu-estimated keypoints * 'naive_gt_kps': naive triangulation keypoints * 'pose_2d_l': human 2d keypoints from left camera * 'pose_2d_r': human 2d keypoints from right camera * 'radar_avail_frames': available frames for radar-estimated keypoints * 'radar_est_kps': radar-estimated keypoints * 'refined_gt_kps': refined triangulation keypoints ground truth * 'rgb_avail_frames': available frames for rgb-estimated keypoints * 'rgb_est_kps': rgb-estimated keypoints * 'video_label': video action labels ***feature*** folder contains imu, radar features for deep learning models. The features are generated from the synced data. * For radar: each folder subject* contains a .npy file subject*_featuremap.npy: * Dimension of the radar feature is (frames, 14, 14, 5). The final 5 means x, y, z-axis coordinates, Doppler velocity, and intensity. * For imu: each folder subject* contains seven files: * acc.pt: acceleration torch data * ori.pt: orientation torch data * acc_ori.pt: acceleration and orientation torch data * Dimension of the radar feature is (frames, 6, 12). 6 is the number of IMUs and 12 is flattened 3x3 rotation and 3 accelerations. * IMU*.csv: IMU raw data. The meaning of header is explained in previous Tabular header section. ***model*** folder contains the pretrained model .pkl files and and results. ## Sharing/Access information Links to other publicly accessible locations of the data: * [Github repo](http://github.com/sizhean/mri) ## Reference ``` @article{an2022mri, title={mri: Multi-modal 3d human pose estimation dataset using mmwave, rgb-d, and inertial sensors}, author={An, Sizhe and Li, Yin and Ogras, Umit}, journal={Advances in Neural Information Processing Systems}, volume={35}, pages={27414--27426}, year={2022} } ```

# Access Points
https://datadryad.org/stash/dataset/doi:10.5061/dryad.9ghx3ffpp

# Related Identifiers
## IsCitedBy
- https://doi.org/10.48550/arxiv.2210.08394