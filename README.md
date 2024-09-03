
### How to run this code?

**Step 1:** Create a directory in your local machine and cd into it

```
mkdir ~/Desktop/opencv_project
cd ~/Desktop/opencv_project
```

**Step 2:** Clone the repository and cd into the folder:

```
git clone [https://github.com/Jaswanth113/Object-Detection.git]
cd Object-Detection
```
**Step 3:** Install all the necessary libraries.

```
brew install opencv
pip install opencv-python
pip install opencv-contrib-python
pip install opencv-python-headless
pip install opencv-contrib-python-headless
pip install matplotlib
pip install imutils
```

Ensure you have OpenCV 3.3 or newer with both opencv and opencv-contrib releases for the dnn module.

**Step 4:** Ensure your video devices are connected. List them with the following command:

```
system_profiler SPCameraDataType
system_profiler SPCameraDataType | grep "^    [^ ]" | sed "s/    //" | sed "s/://"
```

**Step 5:** To start your video stream and real-time object detection, run the following command:

```
python real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
```
