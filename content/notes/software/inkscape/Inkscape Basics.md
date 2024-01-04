---
title: Inkscape Basics
feed: show
date: 2023-03-22"
tags:
---

# Cropping an image
1. Create a shape to use to crop
2. ![[notes/software/inkscape/images/ShapeSelector.png]]
3. Position the shape over the image to crop (use transparency controls if needed)
4. ![[notes/software/inkscape/images/masking.png]]
5. Change the mouse back to the selection tool
6. Select both objects and go to Object->Clip->Set Clip
7. ![[notes/software/inkscape/images/setclip.png]]

# Preparing an Image for 3D
1. Convert the image to vectors 
	1. Path-Trace Bitmap
	2. Choose the following settings:
		1. Smooth/Stack/Remove Background
		2. If an outline is desired, choose Optimize. If fill is required, do not choose Optimize
		3. ![[notes/software/inkscape/images/TraceBitmap.png]]
2. Select new vectors, export selected as SVG
3. Move over to [[notes/software/3dmodeling/Blender|Blender]]
### Reference: https://spolearninglab.com/curriculum/software/3d_modeling/blender/blender_02.html