# Autonomous-Road-Lane-detection

Aim:
Autonomous lane etection for Self driving cars.

Video Source:
https://pixabay.com/videos/

Methodology:

1. Capturing & decoding : We will capture the video using VideoCapture object & after capturing, every video frame is decoded into images.
2. Grayscale image conversion : Frames (in RGB format) is converted to grayscale.
3. Reduce noise: Noise can create false edges, hence its reduction is necessary for image polishing. Hence,Gaussian filter is applied.
4. Canny Edge Detector: The canny function computes the derivative in x and y directions, subsequently, changes in intensity value are seen. 
Larger derivatives = High intensity and vice-versa.
5. Region of Interest: Here only region covered by lane of road i accounted for. A mask is created commensurate with the road image taken.  It ultimately masks the canny image and depicts region of interest traced by polygonal contour of mask.
6. Hough Line Transform: The Probabilistic Hough Line Transform is used, which provides output as the extremes of the detected lines. (Basically used to detect straight lines.)


Sample output photo:
![image](https://user-images.githubusercontent.com/86003669/123514365-53982480-d6b0-11eb-92dc-5e7d3f3ad0e9.png)

You can also access the whole output video clearly in the files uploaded.
