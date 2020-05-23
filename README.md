# Multiple-object-detection-api
This repository consists of almost all type of object detection and emerges into single function/ api to handle.

It consists of
+ Optical flow
+ Dense Optical flow
+ Meanshift Tracking
+ Camshift Tracking
+ Single Tracking 
+ Multi Tracking

## Optical flow 
It is the pattern of apparent motion of objects, surfaces, and edges in a visual scene caused by the relative motion between an observer and a scene.Optical flow can also be defined as the distribution of apparent velocities of movement of brightness pattern in an image.

![alt text](https://nanonets.com/blog/content/images/2019/04/single-object-tracking-using-optical-flow.gif)

## Dense Optical Flow
Dense optical flow attempts to give you the flow all over the image - up to a flow vector per pixel.

## Meanshift Tracking
The mean-shift algorithm is an efficient approach to tracking objects whose appearance is defined by histograms. It is not limited to colors.

![alt text](https://docs.opencv.org/master/meanshift_face.gif)

## Camshift Tracking
It is nothing but increasing or decreasing the size  of the windows based on object distance to Cam.It applies meanshift first. Once meanshift converges, it updates the size of the window as, s=2×M00256−−−√. It also calculates the orientation of the best fitting ellipse to it. Again it applies the meanshift with new scaled search window and previous window location. The process continues until the required accuracy is met.

![alt text](https://docs.opencv.org/master/camshift_face.gif)

## Single Tracking 
In Single Object Tracking (SOT), the bounding box of the target in the first frame is given to the tracker. The goal of the tracker is then to locate the same target in all the other frames. This means that Single Object Trackers should be able to track whatever object they are given, even an object on which no available classification model was trained.

![alt text](https://s3-us-west-2.amazonaws.com/static.pyimagesearch.com/opencv-object-tracking/opencv_object_tracking.gif)

## Multi Tracking
In Multiple Object Tracking, as its name indicates, there are multiple objects to track. The tracking algorithm is expected first to determine the number of objects in each frame, and second, to keep track of each object’s identity from one frame to the next.


