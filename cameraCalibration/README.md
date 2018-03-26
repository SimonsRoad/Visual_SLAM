# Pose Estimation and Camera Calibration
In this package, we mainly implement the **Camera Calibration** algorithm for both hand-handle camera and the monocular camera equipped on a real Quadrotor.

Hand-handled Camera Calibration
-------------------------------
We aim to estimate the intrinsic (K) and extrinsic (R, t) matrices for a hand-handled camera using a planer world space(e.g. checkerboard) and multiple views, which is also called as _camera calibration_. 

* _**Data Collection**_           
For the data collection, simply capture multiple images of a planar checkerboard pattern (known 3D points). More specifically, the pipeline shows below:
  *  _Get a checkerboard_         
  You can use a physical checkerboard if you can find one. Alternatively, print out the predeﬁned checkerboard pattern (use open checkerboardPattern.pdf to show the pattern in MATLAB). Note that the checkerboard pattern is made of odd number of squares in one side and even number of squares on the other side to disambiguate the orientation of the pattern.       
  * _Measure Size_    
  Measure the size of your own checkerboard square in mm (just a recommended unit) such that you can obtain the 3D coordinate for every corner in the checkerboard.    
  * _Images Capture_    
  