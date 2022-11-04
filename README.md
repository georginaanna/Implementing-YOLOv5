# YOLOv5
## Computer vision for object detection using YOLOv5

Usage: SageMakerStudioLab (it's free) 

This repo contains a training approach to training the YOLOv5 model on the coco128 dataset using the `_YOLOv5-Custom-Training.ipynb` notebook. The 
`_YOLOv5-Custom-Training.ipynb` notebook clones the latest ultralytics git page in the first code block (https://github.com/ultralytics/yolov5.git) that is up to date as of the 4th November 2022. 
This repo already contains the coco128 dataset, within the `_YOLOv5-Custom-Training.ipynb` the code points to the coco128 folder that contains the data
via a YAML file. The YAML files can be found in the `yolo-files`, the YAML file for the coco128 dataset is called `coco128.yaml`. (Note: the file structure 
of the coco128 dataset is super important here, with one folder called `images`, one folder called `labels` and another called `test` - you can place what 
ever images you would like in this one to test if the YOLOv5 model you have trained from the coco128 dataset can identify objects within the test images you 
have selected. 

Once you have got your head round the above you can create you own folder with your own data like we have done to create a model that can detect potato stems. We put the data in the `my-own-images` folder with the same folder structure as the coco128 folder, a new yaml was created called `my-own-images.yaml` that was placed in the `yolo-files` folder with the other YAML files and a new ipynb file was created called `my_own_images_script.ipynb`

***Note: The `_YOLOv5-Custom-Training.ipynb`and the 'my_own_images_script.ipynb` exist seperatley, you can run them both but you do not need one to run 
the other and vice versa. 



