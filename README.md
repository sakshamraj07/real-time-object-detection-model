# real-time-object-detection-model
# Real-Time-Object-Detection-With-OpenCV

### Introduction

**Real-Time Object Detection with OpenCV**

This project focuses on achieving real-time object detection through a laptop camera or webcam using OpenCV and MobileNetSSD. The objective is to loop through each frame of the video stream, identify objects such as persons, chairs, dogs, etc., and enclose each detection within a bounding box.

**Getting Started**

1. **Clone the Repository:**
   
   ```
   git clone https://github.com/Surya-Murali/Real-Time-Object-Detection-With-OpenCV.git
   cd Real-Time-Object-Detection-With-OpenCV
   ```

2. **Install Necessary Libraries:**

   Ensure you have the required libraries installed. For MacOS, you can use Homebrew and pip to install the necessary dependencies:

   ```
   brew install opencv
   pip install opencv-python
   pip install opencv-contrib-python
   pip install opencv-python-headless
   pip install opencv-contrib-python-headless
   pip install matplotlib
   pip install imutils
   ```

   Make sure to download and install OpenCV and OpenCV-contrib releases for OpenCV 3.3 or newer to ensure the deep neural network (dnn) module is installed.

3. **Verify Video Devices:**

   Check your connected video devices (e.g., webcam, FaceTime HD Camera) by running the following command in your terminal:

   ```
   system_profiler SPCameraDataType
   system_profiler SPCameraDataType | grep "^    [^ ]" | sed "s/    //" | sed "s/://"
   ```

4. **Start Video Stream and Object Detection:**

   Begin your video stream and real-time object detection using the command:

   ```
   python real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
   ```

5. **Additional Help:**

   For assistance regarding the arguments you pass, you can use:

   ```
   python real_time_object_detection.py --help
   ```

**References and Useful Links**

- [MobileNet-SSD GitHub Repository](https://github.com/chuanqi305/MobileNet-SSD)
- [OpenCV GitHub Repository](https://github.com/opencv/opencv)
- [Understanding OpenCV's blobFromImage Function](https://www.pyimagesearch.com/2017/11/06/deep-learning-opencvs-blobfromimage-works/)
- [Imutils GitHub Repository](https://github.com/jrosebr1/imutils)

This project leverages MobileNet-SSD for object detection, OpenCV for image processing, and Imutils for basic image processing functions. It provides a practical implementation of real-time object detection, making it useful for various computer vision applications.
