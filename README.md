# YOLOV3 + EAST 
### Object+Text Detection Tester
![](https://github.com/cca2016/TestingYoloV3/blob/master/jeep_yolo_EAST_py.jpg)

## **Download the model weights and configuration files**
##  For Linux
Run the getModels.sh file from command line to download the needed model files

	sudo chmod a+x getModels.sh
	./getModels.sh

##  For Windows
Download the files from the links given below

https://pjreddie.com/media/files/yolov3.weights  
https://github.com/pjreddie/darknet/blob/master/cfg/yolov3.cfg  
https://github.com/pjreddie/darknet/blob/master/data/coco.names  


## Getting the EAST Model

1. The `text detection` scripts use **EAST Model** which can be downloaded using this link: https://www.dropbox.com/s/r2ingd0l3zt8hxs/frozen_east_text_detection.tar.gz?dl=1

2. Once the file has been downloaded (~85 MB), unzip it using `tar -xvzf frozen_east_text_detection.tar.gz`.

3. After unzipping, copy the **`.pb`** model file to the working directory.

# **Running the code**

## Python:
Commandline usage for object detection using YOLOv3  
a single image: 
>> 
```
python3 object_text_detection.py --image=XXX.jpg 
``` 

a video file: 
>> 
```
python3 object_text_detection.py --video=XXX.mp4  
```