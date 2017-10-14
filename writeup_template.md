# **Finding Lane Lines on the Road** 


**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Extract frames from Video and use pipeline to process the frames and combine the processed frames back into video


1. Describe your pipeline. 

The pipeline consists of 5 steps. Each frame is executed through these steps to convert into the required output

1. Convert to Greyscale -  first step in pipeline is to convert the image into greyscale
2. Gaussian filtering - second step is to do Gaussian filtering for smoothening of image
3. Canny Edge Detection - third step is to do Canny edge detection
4. Set Region of Interest - Fourth step is to set region of Interest, using vertices. Vertices are selected automatically based on the video dimensions.
5. Apply Hough Transformation - Fifth step is to apply Hough transformation and draw line and extrapolate left and right lines separately


2. Identify potential shortcomings with your current pipeline

1. Though, i am selecting the vertices automatically using the Image. shape, this is still not perfect and the application detects lanes incorrectly sometime
2. Need a better algorithm for vertices selection
