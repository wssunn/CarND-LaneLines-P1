# **Project 1 - Finding Lane Lines on the Road** 
---

**Finding Lane Lines on the Road**

The goal of this project is to **make a pipeline that finds lane lines on the road**.


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I used canny edge detection within a specific region. Then lane lines are found in Hough space.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by calculating median gradients for both left and right lanes.

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
