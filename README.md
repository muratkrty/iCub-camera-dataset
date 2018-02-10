
# iCub camera dataset  
[![DOI](https://zenodo.org/badge/120915707.svg)](https://zenodo.org/badge/latestdoi/120915707)  
<p align="justify">
In this technical post,  the detailed description of a new dataset constructed with the iCub humanoid robot platform and a motorized turntable.  To construct a new dataset via a robot platform, we followed similar acquisition procedures used for the Columbia Object Image Library (COIL-100) [1].  In that, we selected 50 different graspable (by a robotic hand) objects. With the robot camera, we captured images of an object performing a full rotation in steps of approximately 5 degrees. In total, we collected 3600 color images of 50 objects (72 per object). 5 objects (a, b, c, d, e) and various rotations of a selected object (e, d, f, g, h) are shown in the  figure below.
<p align="center">
<img src="http://www.crossvalidate.me/assets/objects.png" >
</p>
</p>

### Hardware setup and image acqusition  
<p align="justify">
The acquisition setup consists of the iCub humanoid robot and a motorized turntable. The setup can be seen in the figure below. The data acquisition procedure begins with placing an object on the turntable; the object is, then, rotated by approximately 5 degrees while capturing an image with the iCub’s camera located in the left eye of the robot. The Yet Another Robot Platform (YARP) middleware and its Python binding were used to capture raw image data (RGB pixel matrices). The obtained data were converted to the PNG format. This procedure was repeated until the turntable completes a full rotation. 
</p>
<p align="center">
<img src="http://www.crossvalidate.me/assets/icub.png" >
</p>

<p align="justify">
The motivation for constructing a new dataset is to assess whether a robust feature selection can be achieved in an environment where hardware constraints (such as camera resolution, and inaccuracies in the rotation of the turntable) and environmental noise (e.g. reflections and shadows) exist.
</p>

### Acknowledgments  
We would like to thank Andrea Pratesi, Mariangela Manti, and Taimoor Shah Hassan for their help during various stages of the data acquisition procedure.

## References  
[1] S. A. Nene, S. K. Nayar, and H. Murase, "Object image library (coil- 100)," Tech. Rep., 1996.
