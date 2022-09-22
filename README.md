# YOLO OBJECT DETECTION ON JETSON NANO

### Hardware Requirements!
1. Nvidia Jetson nano kit
2. USB camera/CSI camera
3. Ethernet/wifi connection
4. External Monitor/Display
5. 32GB MicroSD Card
6. HDMI Cable
7. Power Adapter with Supply

### Setting up YOLO-Object Detection
1. We will be installing Darknet using the Jetson's terminal from [AlexeyAB/darknet](https://github.com/AlexeyAB/darknet.git).
 ```
 git clone https://github.com/AlexeyAB/darknet.git
 cd darknet
 ```
 
2. Enable GPU and OpenCV support by editing the Makefile and also compile the makefile-
 ```
 sudo nano Makefile
 ```
   Set the following values to enable GPU and OpenCV support-
 >  GPU=1
 
 >  CUDNN=1
 
 >  OPENCV=1

 ```
 make
 ```

3. To run object detection with Darknet, we need a model config and model weights(in the cfg directory).
 ```
 wget https://pjreddie.com/media/files/yolov3.weights
 wget https://pjreddie.com/media/files/yolov3-tiny.weights
 ```

4. We are done with installation part and we need to run the camera module to see the predictions in real time-
 ```
 detectnet-camera.py
 ```


## Live Detection on Jetson Nano Developer Kit


https://user-images.githubusercontent.com/67280548/191699209-1d1a3ad2-1b74-4523-9e25-1e644a4f799b.mp4

