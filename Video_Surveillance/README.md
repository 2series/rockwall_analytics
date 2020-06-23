# Intelligent Video Surveillance
## 21/06/220

Surveillance security is a very tedious and time-consuming job. In this usecase, we'll build a system to automate the task of analyzing video surveillance. We'll analyze the video feed in real-time and identify any abnormal activities like violence or theft

There is a lot of research going on in the industry about video surveillance among them; the role of CCTV videos has overgrown. CCTV cameras are placed all over these days in many cities and towns for surveillance and security

In the last decade, there have been advancements in deep learning algorithms for deep surveillance. These advancements have shown an essential trend in deep surveillance and promise a drastic efficiency gain. The typical applications of deep surveillance are

+ theft identification
+ violence detection
+ detection of the chances of explosion

## Network Architecture

We have generally seen deep neural networks for computer vision, image classification, and object detection tasks. In this project, we have to extend deep neural networks to 3-dimensional for learning spatio-temporal features of the video feed

For this video surveillance usecase, we'll introduce a spatio temporal autoencoder, which is based on a 3D convolution network. The encoder part extracts the spatial and temporal information, and then the decoder reconstructs the frames. The abnormal events are identified by computing the reconstruction loss using Euclidean distance between original and reconstructed batch

![fig1](https://drive.google.com/uc?export=view&id=1ZMiNzAPul7J1m8MQMwbk-rayoArX9hF4)

## The Dataset

**CUHK Avenue Dataset** contains 16 training and 21 testing video clips. The video contains 30,652 frames in total

![](https://drive.google.com/uc?export=view&id=1i7fzIUxz-oEs8V4uMdoZCQUl51NMrbVz)
