## 3D reconstruction of a scene 
# Motivation and goal
The generation of a realistic virtual world by computer is a hot research topic nowadays. This project is based on the TIP technology [ 1 ] proposed by HORRY to generate different views from a single image. Mainly for scene modelling with traditional boxed features. The aim is to visualise 3D reconstruction of a scene stereo images.

# Algorithms 
1. Algorithm to complete missing images [ 2 ]

   <img width="554" alt="image" src="https://github.com/RuanLinya/Computer-Vision-/assets/133128176/f893ed79-1a95-4cdd-90ec-fc66d3020e2a">

     
Determine which pixel of the area to be repaired should have which colour by using the surrounding pixels of the missing area. Interpolate from outside to inside until all pixels are filled.

2. Image Warp Algorithm [ 3 ]

The image distortion algorithm maps the pixel locations of the output distorted image to the pixel locations in the input image by using a reverse mapping technique.

# Reference
[1] Tour Into the Picture: Using a Spidery Mesh Interface to Make Animation from a Single Image, Youichi Horry, January 1997

[2] https://blog.csdn.net/qq_42771692/article/details/99617861

[3] https://www.mathworks.com/help//visionhdl/ug/image-warp.html
