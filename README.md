# 2Stage-Traffic-Sign-Classifier
Traffic Sign Classifier using YOLO object Detection and CNN classifier

This traffic sign classifier classifies the traffic sign images in two stages. It uses YOLOv3 for object detection and classifies the traffic signs in 4 classes, prohibitory, mandatory, danger and other. The image is croped, prosessed and is given as input to a 26 layered CNN model. The CNN classifies the image into 43 classes.

The YOLOv3 model is a model from darknet and is pretrained on COCO image dataset. For the model to work on traffic signs it was trained on GTSDB dataset for 8000 epochs, and the CNN model was trained on GTSRB for 30 epochs.

# Explanation of the files and folders: 
final_models: This foldercontaines the final trained models, configuration files and text files used during classification.

  |-> category.names: This file containes the 4 categories in which the YOLO classifies the traffic sign.
  
  |-> classes.txt: This file containes the list of 43 classes of traffic signs in which the CNN classifies the Croped traffic signs.
  
  |-> cnn26.h5: This is the trained CNN model.
  
  |-> yolov3.cfg: This is the configuration file for the YOLOv3 model, containing the information of all layers in YOLO
  |-> yolov3.weights: This is the trained YOLOv3 model.
  Due the large file size, the two models are not uploaded to the Github repository, these two files can be obtained from https://drive.google.com/file/d/1TuQ3mib2u4MDKnL_uyQtXg0hvG_CFkze/view?usp=sharing
