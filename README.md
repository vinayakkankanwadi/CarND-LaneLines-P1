# **Finding Lane Lines on the Road** 
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

<img src="examples/laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

Overview
---

When we drive, we use our eyes to decide where to go.  The lines on the road that show us where the lanes are act as our constant reference for where to steer the vehicle.  Naturally, one of the first things we would like to do in developing a self-driving car is to automatically detect lane lines using an algorithm.

In this project you will detect lane lines in images using Python and OpenCV.  OpenCV means "Open-Source Computer Vision", which is a package that has many useful tools for analyzing images.  

Goals
---
- P1.ipynb  - pipeline that finds lane lines on the road [code](https://github.com/vinayakkankanwadi/CarND-LaneLines-P1/blob/lane/P1.ipynb)
- README.md - written report to reflect the work [writeup](https://github.com/vinayakkankanwadi/CarND-LaneLines-P1/blob/lane/README.md)

Reflection
---

Lane Finding Pipeline
---

Potential Shortcomings
---
This pipeline works on all the provided sample data. The current pipeline is limited to detecting only the left and right bounds of the current lane. It cannot detect the curvature for a curved road. The other shortcoming is, if the lane lines are not detected for a few frames (due to missing lane lines or traffic), the moving average might yield a wrong result.

Possible Improvements
---
The pipeline can be improved to detect the curvature of the lane along with the bounds. Also, better regression model can be applied to identify missing data instead of using simple moving average to extrapolate missing lane lines.
