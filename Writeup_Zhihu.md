#**Finding Lane Lines on the Road** 

##Writeup Template

###You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report



### Reflection

###1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

Covert RGB image to gray scale image.

Use Gaussian Blur to smooth the image.

Run the Canny edge detection.

Convert the edge to Hough space.

Define a mask function.

Average the lines from Hough output lines.

Draw the lane on the image



###2. Identify potential shortcomings with your current pipeline

- Algorithm shortcomings:

-- The masking parameters are just defined as fixed varibles.

-- Code Engineering shortcomings:

- The varibles are passed through the frames are global variables. These will cause unexpected troubles in debugging in the future.


###3. Suggest possible improvements to your pipeline

- The challenge video is not working for the current algorithm
- Dynamic masking function.
- Fitting 3 degree ploynomial line functions from Hough lines output