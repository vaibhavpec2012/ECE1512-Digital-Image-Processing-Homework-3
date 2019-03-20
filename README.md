# ECE1512_Assignment-3
Lane Detection using Image Segmentation - Berkeley BDD 100K Dataset


The purpose of the code is to create an effective lane marking algorithm that can be used by an autonomous vehicle so that it can understand the content in the images and thius make informed decisions.

**ENet** was chosen as the algorithm for the purpose becuase it claims to provide the same accuracy as well known models such as FCN and UNet while having 2 orers less of trainabel parameters.

Two models are created with the same Enet architecture:

-  One is trained on RGB images
-  The other is trained on Canny Equivalent of images. This has been done to reduce the information that the model needs to process.

Masks were created by plotting the nodes provided for Bezier Curve in the 'poly2D' key of the Labels Json.

The model was able to achieve a Mean IoU of ~0.7 on the validation and testing set. The Model was evaluated for a video and various images for different working conditions  
