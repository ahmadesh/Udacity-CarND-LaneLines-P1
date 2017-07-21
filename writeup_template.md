# **Finding Lane Lines on the Road** 

<img src="examples/laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

Overview
---

### Description of the pieline:

My pipeline consisted of the following steps.

1- Conversion to grayscale

2- Masking the grayscale image with white and yellow color masks

3- Gaussian blur with kernel 5

4- Canny edge detection

5- Region of interest masking

6- Hough transform and draw-line() function to detect the left and right lines and drawing them on the image 

7 - Overlaying the line image on original image.

The drawline() function takes the Hough lines and:

* Separates the left and right lines coordinates based on thier slopes. In case no left or right line is detected, or variance of the line slopes is abnormal, the function returns the lines from previous frame.
* Fits a first order polynomial (line) over the coordinates (x,y) of the left and right Hough lines.
* Calculates the coordinates of the continues left and right lines based on the fit parameters.
* Combines the line coordinates of the current frame (previous step) with the previous frame with a ratio.
* Adds the left and right lines to a blank image 

Description of the pieline:



### Test on images:
First, the pipeline is tested on sample images. A sample of the input images is:

![alt text][image1]

### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
