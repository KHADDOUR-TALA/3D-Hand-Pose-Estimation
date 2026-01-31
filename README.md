# 3D Hand Pose Estimation from Stereo Camera
This project implements a 3D hand pose estimation pipeline using stereo cameras.
It reconstructs 3D hand keypoints by triangulating 2D detections using Direct Linear Transformation (DLT). It supports three different 2D hand keypoint detectors for triangulation:
## OverView 
- Uses **stereo camera** input to estimate 3D hand pose

- Supports multiple 2D hand keypoint detectors:

- **Mediapipe**
- **RTMPose**
- **LiteHRNet**

- Includes **fisheye camera distortion** modeling to improve accuracy

- Designed as part of the **MirrorGlove** system for hand motion mirroring

## Tools & Technologies

1. Python

2. OpenCV

3. PyTorch

4. Mediapipe

5. MMPOSE
   
This video shows the 2D keypoints of running Mediapipe and the 3D plots of each model for the same input (RTMPose, Mediapipe, and LightHRNet respectively)
<div align="center">
  <video src="https://github.com/user-attachments/assets/71ac803b-e8d6-4938-b31f-57551a7a09c4" autoplay loop muted playsinline></video>
</div>

## Usage

1. Calibrate the stereo cameras and place parameters in 'src/camera_parameters/'

2. Run one of the models:

 - Mediapipe3D.py (real-time)

 - RTMPose3D.py or LiteHRNet3D.py (video input)

 - View 2D keypoints, 3D plots, and saved output files

## Results

**Distortion modeling improves 3D accuracy

**Lower MPJPE when fisheye distortion is modeled

**Filtering reduces noise in reconstructed 3D trajectories
## Authors
 - Tala Khaddour
 - Alaa Hassoun
 - Aya Sadek
 - Zain Soliman

