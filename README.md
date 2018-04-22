# Face-Detection
The goal is to detect faces through webcam using Haar Feature-based Cascade Classifiers

# Method
Viola – Jones algorithm is used. This object detection method was proposed by Paul Viola and Michael Jones in their paper, "Rapid Object Detection using a Boosted Cascade of Simple Features" in 2001. It is a machine learning based approach where a cascade function is trained from a lot of positive images (instances of the object class of interest) and negative images (images that don’t contain the object of interest).  It is then used to detect objects in other images.

OpenCV library comes with a trainer as well as detector. OpenCV already contains many pre-trained classifiers for face, eyes, smiles, etc that work on grayscale images. These XML files are stored in the opencv/data/haarcascades/ folder.

A Function detect(gray, frame) is created that takes as input the image in black and white (gray) and the original image (frame), and returns the original image with the detector rectangles. 
For computational efficiency, face detection is done on the global referential whereas eyes & smile detection is done inside the referential of the face.

