# indian-food-instance-segmentation

## ABOUT
</p>
  For the purpose of this project, I am developing an instance segmentation model that can detect multiple Indian food dishes in a plate through a single image. The performance of two models, YOLOv8 and Detectron2, are compared to identify the best fit. <br />

## DATASET
A custom dataset was prepared by scraping images of the most common Indian food items using DuckDuckGo Image Search API. <br />

The images were then annotated using Roboflow, a comprehensive platform that allows developers to easily create and pre-process custom datasets and also build and deploy computer vision models. <br />

Link to dataset: [https://universe.roboflow.com/internship-cjnh4/neuroequilibrium-internship/dataset/2](https://universe.roboflow.com/internship-cjnh4/neuroequilibrium-internship/dataset/2)

</p>

## SEGMENTATION
Image segmentation refers to the task of identifying and classifying multiple categories of objects in an image. Image classification assigns a single class to the whole image, but here the requirement is to detect multiple classes (food items) within a single image. Hence, image segmentation is important.

<img alt="Image Segmentation" src="https://github.com/aarshroongta1/internship-indian-food-segmentation/assets/108404307/f6eb2013-eda5-4d4a-a3b7-30e6bbd285c9" width="300">
</br>
The two common types of segmentation are:

  ### Semantic Segmentation
  In semantic segmentation, all the objects that belong to the same class share the same label. 

  ### Instance Segmentation
  Instance segmentation goes a step further by assigning a unique label to each distinct instance of the class. This is relevant when finding out the number of objects even within the same class. <br />

  Now consider the following image:

<img alt="Instance Segmentation" src="https://github.com/aarshroongta1/internship-indian-food-segmentation/assets/108404307/9aaa8b12-a050-4226-a90e-07790fa56ed2" width="300">

As can be observed, every Gulab Jamun (Indian sweet) is detected separately, so we know that the user is consuming four of these and the calorie and sugar levels can be logged accordingly.

## RESULT
<p>
  The mAP-50 (mean Average Precision at an IoU threshold of 0.5) obtained for YOLOv8 and Detectron2 are approximately 80% and 35%, respectively. <br />

Hence, this proof of concept has helped decide that a YOLOv8 model can be used for a similar project to be conducted using a much larger and diverse dataset.

</p>
