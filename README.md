# VideoAnalysis

Update: 2025
This was a test project that I am building with the Jetson Nano to try to detect my daughter during her soccer matches.  The goal was to have it do object detection and tracking so that I could put a bounding box to extract the parts of the videos that she was in.  The intent was to build highlights for college coaches.  

This was a Covid project.

This is the sample code for the soccer tracking project

This will initially be a montage of the concepts that I am learning as I try to realize this project

The example is derived from this post: https://www.pyimagesearch.com/2019/06/10/keras-mask-r-cnn/

This uses the Mask R-CNN implementation from Matterport :https://github.com/matterport/Mask_RCNN
I had to fix this to use the current libraries and methods so I forked it: https://github.com/hivie7510/Mask_RCNN
After cloned, run setup.py install

Create new python environment
conda create -p ./vaenv python=3.6.8

Activate the environment
conda activate /Users/hivie/Projects/VideoAnalysis/vaenv

Install dependencies
pip install numpy scipy
pip install pillow scikit-image matplotlib imutils
pip install "IPython[all]"
pip install tensorflow
pip install keras h5py
pip install opencv-contrib-python

I had a lot of problems with the environment stuff since I am a noob with python, so I learned the hard way to check
if you can import the opencv and tensorflow modules

This is the graph that I used faster_rcnn_inception_resnet_v2_atrous_oid_v4_2018_12_12

