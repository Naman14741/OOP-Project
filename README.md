# OOP Project
A mini face detection project using OpenCV Java.

1. In YuNet.java I used a Face Detection YuNet model, which I also provided the raw version to download in the `/resources` directory.

2. All related models are stored in the `models` directory.

## Notes
Running the `FaceDetectorYN.detect(Mat image, Mat faces)` returns a 2D cv::Mat of shape [num_faces, 15]:
- 0-1: x, y of bbox top left corner 
- 2-3: width, height of bbox 
- 4-5: x, y of right eye 
- 6-7: x, y of left eye 
- 8-9: x, y of nose tip 
- 10-11: x, y of right corner of mouth 
- 12-13: x, y of left corner of mouth  
- 14: face score

For more information, see: https://docs.opencv.org/4.x/javadoc/org/opencv/objdetect/FaceDetectorYN.html#detect(org.opencv.core.Mat,org.opencv.core.Mat)
