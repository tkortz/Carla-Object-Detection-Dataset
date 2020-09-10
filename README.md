# Carla-Object-Detection-Dataset
Labeled Dataset for Object Detection in Carla Simulator

This dataset contains 1628 images, each 640x380 pixels. The dataset is split into 328 test and 1300 training examples.  It can be used to train a [vehicle and pedestrian detector](https://github.com/tkortz/Tensorflow-Carla-Object-Detection).

Every image comes with an associated label .xml file in the pascal VOC format. The dataset was collected in Carla Simulator, driving around in autopilot mode in various environments (Town01, Town02, Town03, Town04, Town05) and saving every x frame. The labels where then automatically generated using the semantic segmentation information. 

Available classes are: 

* Vehicle (Car, Truck)
* Bike
* Motobike
* Pedestrian

The original repository also contained labels for the following classes:

* Traffic light
* Traffic sign

Thus, the original 1028 .xml files (208 test, 820 training) contain labels for traffic lights and traffic signs, but the new 600 .xml files (120 test, 480 training) do not.  Additionally, the original files do not contain any pedestrians.

Example image:

![example image](https://github.com/tkortz/Carla-Object-Detection-Dataset/blob/master/test/Town01_011940.png "Example Image from Dataset")

