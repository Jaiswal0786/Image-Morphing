Image Morphing->
This program takes in two images and uses morphing techniques to create a sequence of intermediate images that
seamlessly transition from one image to the other. The resulting sequence is saved as an animated GIF.

Requirements:->
Python 3.5+
OpenCV
Numpy
dlib
scipy
imageio

Usage:->
Place the two input images in the same directory as the script.
Run the script.
The resulting animated GIF will be saved in the same directory.

How it Works:->
The program works by first detecting facial landmarks in each input image. These landmarks are then used to create 
a Delaunay triangulation, which defines a set of triangles that cover the entire face. For each pair of 
corresponding triangles in the two input images, a morphing function is applied to blend the two images together. 
The process is repeated for a range of alpha values, which determine the degree of blending between the two images. 
The resulting sequence of intermediate images is then combined into an animated GIF.