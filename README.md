# indian-food-instance-segmentation

## ABOUT
</p>
  For the purpose of this project, I am developing an instance segmentation model that can detect multiple Indian food dishes in a plate through a single image. The performance of two models, YOLOv8 and Detectron2, are compared to identify the best fit. <br />

## DATASET
A custom dataset was prepared by scraping images of the most common Indian food items using DuckDuckGo Image Search API. <br />

The images were then annotated using Roboflow, a comprehensive platform that allows developers to easily create and pre-process custom datasets and also build and deploy computer vision models. <br />

Link to dataset: [https://universe.roboflow.com/internship-cjnh4/neuroequilibrium-internship/dataset/2](https://universe.roboflow.com/internship-cjnh4/neuroequilibrium-internship/dataset/2)

</p>

## RESULT
<p>
  The mAP-50 (mean Average Precision at an IoU threshold of 0.5) obtained for YOLOv8 and Detectron2 are approximately 80% and 35%, respectively. <br />

Hence, this proof of concept has helped decide that a YOLOv8 model can be used for a similar project to be conducted using a much larger and diverse dataset.

</p>
