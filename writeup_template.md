# **Finding Lane Lines on the Road** 

The goals of this project is to make a pipeline that finds lane lines on the road.

[//]: # (Image References)

---

### 1. Description of the pieline:

My pipeline consisted of the following steps.

1- Conversion to grayscale
2- Masking the grayscale image with white and yellow color masks
3- Gaussian blur with kernel 5
4- Canny edge detection
5- Region of interest masking
6- Hough transform and draw-line() function to detect the left and right lines and drawing them on the image 
7 - Overlaying the line image on original image.


![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
