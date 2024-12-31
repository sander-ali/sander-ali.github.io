---
layout: post
title: "Taking a Deep Dive into YOLOv8"
description: "Details on YOLOv8"
date: 2023-08-03 09:00:00-0400
tags: [YOLOv8, Python, Github, Object Detection, Object Segmentation]
thumbnail: assets/img/blog/YOLOv8_dive_2023.PNG
---

Ultralytics unveiled YOLOv8 on January 10, 2023, which has garnered over one million downloads since its debut. This blog post aims to delve into the intricacies of YOLOv8.


## What is YOLOv8

YOLOv8 is the latest cutting-edge YOLO model, designed for object detection, image classification, and instance segmentation tasks. Developed by Ultralytics, the creators of the influential YOLOv5 model, YOLOv8 incorporates several architectural and developer experience enhancements compared to its predecessor. Currently, YOLOv8 is in active development as Ultralytics continues to introduce new features and address community feedback. It is worth noting that Ultralytics provides long-term support for their models, collaborating with the community to optimize the model's performance.

## HOW YOLO Grew Into YOLOv8

The YOLO (You Only Look Once) series of models has gained significant recognition in the field of computer vision. YOLO's popularity stems from its impressive accuracy despite having a compact model size. This attribute allows YOLO models to be trained efficiently on a single GPU, making it accessible to a diverse community of developers. Machine learning practitioners can deploy YOLO models at a low cost, either on edge hardware or in the cloud. For a concise overview of the timeline of YOLO models, please refer to my other article.

{% include figure.liquid loading="eager" path="assets/img/blog/YOLOv8_dive_2023.png" class="img-fluid rounded z-depth-1" %}

## Why Should you use YOLOv8

There are several compelling reasons to consider using YOLOv8 for your next computer vision project:

1. YOLOv8 offers improved accuracy compared to previous YOLO models.

2. The latest YOLOv8 implementation includes a range of new features, such as a user-friendly CLI and a GitHub repository.

3. YOLOv8 supports various tasks, including object detection, instance segmentation, and image classification.

4. The YOLO community is highly active and supportive, with numerous tutorials, videos, and articles available. You can also find assistance in communities like MLOps Community and DCAI.

It's worth noting that training YOLOv8 is likely to be faster than other two-stage object detection models. However, there is one limitation to consider: YOLOv8 does not currently support models trained at a resolution of 1280 pixels. Therefore, if you require high-resolution inference, it is not recommended to use YOLOv8.

In addition to its performance, YOLOv8 offers significant developer-convenience features. Unlike other models that spread tasks across multiple Python files, YOLOv8 provides a CLI that simplifies the model training process. Moreover, the Python package accompanying YOLOv8 ensures a smoother coding experience compared to previous models.

The YOLO community's expertise and extensive online resources also make it an attractive choice. Many computer vision experts are familiar with YOLO and can provide guidance. Although YOLOv8 is relatively new, there is already a wealth of online guides available to assist users.


## How does YOLOv8 compare to previous models?

The Ultralytics team has recently conducted a benchmark of YOLOv8 using the COCO dataset, yielding impressive results when compared to previous versions of YOLO across all five model sizes. In evaluating the performance of different YOLO lineages and model sizes on the COCO dataset, they used various metrics for the assessment. These include performance (mean average precision or mAP), speed of inference (measured in frames per second or fps), and compute cost (represented by the size of the model in terms of FLOPs and parameters).

{% include figure.liquid loading="eager" path="assets/img/blog/Dive_YOLOv8_1.jpg" class="img-fluid rounded z-depth-1" %}

In the object detection comparison of the five model sizes, the YOLOv8m model achieved an mAP of 50.2 % on the COCO dataset, while the largest model, YOLOv8x, achieved a higher mAP of 53.9 % with more than double the number of parameters.

{% include figure.liquid loading="eager" path="assets/img/blog/Dive_YOLOv8_2.jpg" class="img-fluid rounded z-depth-1" %}

Overall, YOLOv8 demonstrates exceptional accuracy and performance, positioning it as a compelling choice for your next computer vision project. Whether you are considering implementing object detection in a commercial product or exploring the latest advancements in computer vision, YOLOv8 stands as a cutting-edge model worth considering. For a brief tutorial of YOLOv8 by Ultralytics, we invite you to check out their colab tutorial [https://medium.com/r/?url=https%3A%2F%2Fcolab.research.google.com%2Fgithub%2Fultralytics%2Fultralytics%2Fblob%2Fmain%2Fexamples%2Ftutorial.ipynb].


## YOLOv8 Architecture: A Deep Dive

The layout presented by RangeKing on GitHub [https://medium.com/r/?url=https%3A%2F%2Fgithub.com%2Fultralytics%2Fultralytics%2Fissues%2F189] is an excellent visualization of the architecture. Although YOLOv8 does not currently have a published paper, which limits our direct understanding of the research methodology and ablation studies conducted during its development, we can still analyze the code and repository to gather information about the model. By documenting the distinctions between YOLOv8 and other architectures, we can gain insights into its unique features.

{% include figure.liquid loading="eager" path="assets/img/blog/dive_YOLOv8_3.jpg" class="img-fluid rounded z-depth-1" %}

## New convolutions in YOLOv8

According to the introductory post from Ultralytics, the YOLOv8 architecture has undergone a series of updates and new modifications. Here are the key changes:

>> The backbone of the system has been altered by replacing C3 [https://github.com/ultralytics/yolov5/blob/cdd804d39ff84b413bde36a84006f51769b6043b/models/common.py#L157] with C2f [https://github.com/ultralytics/ultralytics/blob/dba3f178849692a13f3c43e81572255b1ece7da9/ultralytics/nn/modules.py#L196]. In the stem, the first 6x6 convolution has been replaced with a 3x3 convolution. In C2f, the outputs from the Bottleneck (which consists of two 3x3 convolutions with residual connections) are combined, whereas in C3, only the output from the last Bottleneck was utilized.

>> Two convolutions (#10 and #14 in the YOLOv5 configuration) have been eliminated.

>> The Bottleneck in YOLOv8 remains the same as in YOLOv5, except for the change in the kernel size of the first convolution from 1x1 to 3x3. This adjustment indicates a shift towards the ResNet block defined in 2015.

{% include figure.liquid loading="eager" path="assets/img/blog/dive_YOLOv8_4.png" class="img-fluid rounded z-depth-1" %}

## Anchor Free Detection

YOLOv8 is a model that does not rely on anchor boxes. Instead, it directly predicts the center of an object without considering the offset from a pre-defined anchor box.

{% include figure.liquid loading="eager" path="assets/img/blog/dive_YOLOv8_5.png" class="img-fluid rounded z-depth-1" %}

## Anchor Boxes

In previous versions of YOLO, anchor boxes posed a challenge as they may not accurately represent the distribution of object boxes in a custom dataset, but rather the distribution of object boxes in a general benchmark dataset. 

By adopting an anchor-free approach, the number of box predictions is reduced, resulting in faster Non-Maximum Suppression (NMS). NMS is a complex post-processing step that filters through candidate detections after the inference process.

## Closing the Mosaic Augmentation

Deep learning research often prioritizes the development of model architecture; however, in the case of YOLOv5 and YOLOv8, the training routine plays a crucial role in their success. During training, YOLOv8 employs online augmentation, which involves presenting the model with slightly different variations of the provided images at each epoch. One of these augmentations is known as mosaic augmentation, where four images are stitched together. This forces the model to learn about objects in new locations, partial occlusion, and against varying surrounding pixels.

Nevertheless, it has been empirically observed that if mosaic augmentation is applied throughout the entire training routine, it can lead to a decline in performance. Thus, it is advisable to disable this augmentation for the last ten training epochs. This modification exemplifies the meticulous attention given to YOLO modeling over time in both the YOLOv5 repository and the YOLOv8 research.

## Implementing YOLOv8

Let's examine the utilization and implementation of YOLOv8 in your workflows. YOLOv8 includes pre-trained models that can be readily employed in your computer vision projects to enhance model performance. These models consist of instance segmentation models trained on the COCO segmentation dataset with an image resolution of 640, image classification models pre-trained on the ImageNet dataset with an image resolution of 224, and object detection models trained on the COCO detection dataset with an image resolution of 640.


{% include figure.liquid loading="eager" path="assets/img/blog/dive_YOLOv8_6.jpg" class="img-fluid rounded z-depth-1" %}

## How do I use the YOLOv8 CLI?

YOLOv8 can be accessed easily via the CLI and used on any type of dataset.

```shell
!yolo task=detect \ mode=predict \ model=yolov8n.pt \ source="image.jpg"
```

To use it simply insert the following commands:

- task in [detect, classify, segment]

- mode in [train, predict, val, export]

- model as an uninitialized .yaml or as a previously trained .pt file

Source as the path/to/data

## Can I pip install YOLOv8?

In addition to the CLI, YOLOv8 is available as a PIP package [https://pypi.org/project/yolov8/], making it suitable for Python environments. While this may present some challenges for local development, it provides the flexibility to seamlessly integrate YOLOv8 into your Python code, opening up a wide range of possibilities.

You can clone it from GitHub:

```shell
git clone https://github.com/ultralytics/ultralytics.git
```
or pip install from pip:


```shell
pip install ultralytics
```

After you have installed the package, you can import a model and use it in your choice of python environment:

```shell
from ultralytics import YOLO 

# Load a model
model = YOLO("yolov8n.pt")  # load a pretrained model

# Use the model
results = model.train(data="coco128.yaml", epochs=5)  # train the model
results = model.val()  # evaluate model performance on the validation data set
results = model("https://ultralytics.com/images/cat.jpg")  # predict on an image
success = YOLO("yolov8n.pt").export(format="onnx")  # export a model to ONNX
```

You can also access YOLO models via TensorFlow 2, Keras API, Ultralytics Google Colab Notebook [https://colab.research.google.com/github/ultralytics/ultralytics/blob/main/examples/tutorial.ipynb], and OpenCV [https://opencv-tutorial.readthedocs.io/en/latest/yolo/yolo.html].

## What is the Annotation Format of YOLOv8?

YOLOv8 utilizes a straightforward annotation format that aligns with the YOLOv5 PyTorch TXT annotation format. This format is a modified version of the Darknet annotation format.

For each image sample, there is a corresponding .txt file that contains one line per bounding box. The format for each row is presented as follows:

```shell
class_id center_x center_y width height
```
The coordinates are normalized from 0 to 1 and each field is space delimited. An example of annotation format is shown below:

```shell
1:  1 0.317 0.30354206008 0.114 0.173819742489
2:  1 0.694 0.33726094420 0.156 0.23605150214
3:  1 0.395 0.32257467811 0.13 0.195278969957
```
The model uses the information concerning image location along with class ids and labels from data.yaml folder. The structure of the folder is shown below:

```shell
train: ../train/images
test: ../test/images
val: ../valid/images

nc: 5
names: ['fish', 'cat', 'person', 'dog', 'shark']
```

## Conclusion

To begin implementing YOLOv8 for your own specific use case, please refer to the article/blog [https://learnopencv.com/train-yolov8-on-custom-dataset/] on training YOLOv8 with a custom dataset.

For additional insights and ideas, you can explore Github repositories [https://github.com/keremberke/awesome-yolov8-models], where you will find various YOLOv8 models, datasets, and sources of inspiration.

If you are a practitioner who is actively deploying their model and employing active learning strategies to continuously enhance its performance, many articles/blogs introduce a pathway that allows you to deploy your YOLOv8 model [https://pub.towardsai.net/step-by-step-guide-on-deploying-yolo-model-on-fast-api-fcc6b60f5c26]. This will enable you to utilize our inference engines and benefit from label assist functionality on your dataset.

I wish you success in your training endeavors and productive inference sessions!