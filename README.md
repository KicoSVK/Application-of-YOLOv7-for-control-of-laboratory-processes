# Application of YOLOv7 for control of laboratory processes
This work deals with the problem of detection and evaluation of the pipetting process. The entire system is based on the use of a camera, respectively the camera of a mobile device or tablet, which is conveniently positioned to capture the scene being captured. All image processing, object detection using the {YOLOv7 (You Only Look Once 7. version)} model and subsequent other operations are performed on a mobile device or tablet. The YOLOv7 neural network model was trained on our own prepared dataset. This training set was created specifically for the analysis of the pipetting process. The result of this work is a prepared annotated dataset and a trained YOLOv7 neural network model, which is aimed at detecting the entire pipette and the tip of this pipette in the image scene. The output of the work is also an implemented algorithm that can perform a complex analysis of the pipetting process using the trained YOLOv7 model.

<b>The dataset, scripts and other files used in this work can be found at:</b></br>
https://drive.google.com/drive/folders/1pCiBqvItr4K8-zJZ3WTG0lvnNh--s22S?usp=sharing

<b>To start training neural network model YOLOv4 with framework darknet:</b></br>
<code>sudo path/to/darknet detector train "coco.data" "yolov4-obj.cfg" "yolov4.conv.137" -dont_show -mjpeg_port 8090 -map</code>

<b>To start testing inference of learned neural network model YOLOv4:</b></br>
<code>python3 opencv_yolov4_inference_test.py --video=./video/cars.mp4</code>

<b>Model training results:</b>
<p float="center">
  <img src="https://drive.google.com/uc?id=1dp1jt9ALL_nuU_jnZwyNFSQzIr7gsMcd" width="450" />
</p>

<p float="center">
  <img src="https://drive.google.com/uc?id=1rSnwwOM7-kvNuHolyzvFvrJOlRvSQqER" width="650" />
</p>
