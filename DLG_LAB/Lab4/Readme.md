# Object Detection Using EfficientDet-D7 and R-CNN

## Aim
To detect and classify objects in images using two approaches: EfficientDet-D7 and R-CNN with VGG16 and Selective Search.

## Dataset Used
- **EfficientDet-D7:** Pre-trained model using the COCO 2017 dataset, supporting 80 object categories.
- **R-CNN with VGG16:** Pre-trained VGG16 model using ImageNet, with Selective Search for region proposals.
- **Input:** User-uploaded images, including AVIF format.

## Results
- **EfficientDet-D7:** Detected objects using bounding boxes and confidence scores above 0.5.
- **R-CNN:** Generated 200 region proposals and identified 6 regions labeled as `cab`, using a confidence threshold above 90% and Non-Maximum Suppression (IoU threshold of 0.3).

Both approaches demonstrate object detection and classification using deep learning and computer vision techniques.