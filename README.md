# **Project 1 - Finding Lane Lines on the Road** 
---

The goal of this project is to **make a pipeline that finds lane lines on the road**.


[//]: # (Image References)

[image2]: ./test_images/solidWhiteCurve.jpg "Before"
[image3]: ./test_images_output/solidWhiteCurve.jpg "After"

---

### Reflection

### 1. Description of my pipeline

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I used canny edge detection within a specific region. Then lane lines are found in Hough space.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by calculating median gradients for both left and right lanes.

The unprocessed image is shown below:
![alt text][image2]

Here is the processed one:
![alt text][image3]

### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when white line is too small. Algorithms will fail to detect it or will not be stable.

Another shortcoming could be when the ground suddenly changes colour (becomes whiter). The algorithm could give very unstable output.


### 3. Possible improvements

A possible improvement would be to fine tune the parameters so that the output is more stable.

Another way is to introduce more filters to increase the robustness of the system.
