## 3D reconstruction of a scene 
# Motivation and goal
The generation of a realistic virtual world by computer is a hot research topic nowadays. This project is based on the TIP technology [ 1 ] proposed by HORRY to generate different views from a single image. Mainly for scene modelling with traditional boxed features. The aim is to visualise 3D reconstruction of a scene stereo images.

# Algorithms 
1. Algorithm to complete missing images [ 2 ]

   <img width="554" alt="image" src="https://github.com/RuanLinya/Computer-Vision-/assets/133128176/f893ed79-1a95-4cdd-90ec-fc66d3020e2a">

     
Determine which pixel of the area to be repaired should have which colour by using the surrounding pixels of the missing area. Interpolate from outside to inside until all pixels are filled.

2. Image Warp Algorithm [ 3 ]

   <img width="528" alt="image" src="https://github.com/RuanLinya/Computer-Vision-/assets/133128176/fdd034c4-abb2-45f0-aeb2-168f9d6625d4">


The image distortion algorithm maps the pixel locations of the output distorted image to the pixel locations in the input image by using a reverse mapping technique.

# Principles
1. Extraction of foreground objects

<img width="476" alt="image" src="https://github.com/RuanLinya/Computer-Vision-/assets/133128176/96e34969-056e-4785-92ea-bf6199dd448b">

2. The spider web in TIP technology consists of vanishing point, inner window and outer window.

<img width="160" alt="image" src="https://github.com/RuanLinya/Computer-Vision-/assets/133128176/89184fc4-db85-4a05-94e0-83e929f25e5a">

3. With the help of the lines through the vanishing point and each corner of the rectangle, five walls and the future corners of the room are created. 

<img width="162" alt="image" src="https://github.com/RuanLinya/Computer-Vision-/assets/133128176/1fe3d772-03b2-4ce9-a446-060b59d76fde">

4. Foreground placement

<img width="500" alt="image" src="https://github.com/RuanLinya/Computer-Vision-/assets/133128176/0c3559ad-ac48-4fbf-9619-079f753cc8b7">

5. By function ''meshgrid'' the 3D space is created.

<img width="198" alt="image" src="https://github.com/RuanLinya/Computer-Vision-/assets/133128176/c4064d13-b965-4d9b-b434-f585c4b78ce3">

6. A cube is created by the function ''warp''.  The right wall, left wall, back wall, floor, ceiling are projected onto this BOX model. 

<img width="192" alt="image" src="https://github.com/RuanLinya/Computer-Vision-/assets/133128176/891ed2b6-42f4-4333-bea2-3e193a9d2238">




# Reference
[1] Tour Into the Picture: Using a Spidery Mesh Interface to Make Animation from a Single Image, Youichi Horry, January 1997

[2] https://blog.csdn.net/qq_42771692/article/details/99617861

[3] https://www.mathworks.com/help//visionhdl/ug/image-warp.html
