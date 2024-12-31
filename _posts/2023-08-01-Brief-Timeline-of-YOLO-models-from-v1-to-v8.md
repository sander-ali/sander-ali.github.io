---
layout: post
title: Brief Timeline of YOLO models
description: "Brief Timeline of YOLO models from v1 to v8"
date: 2023-08-01 09:00:00-0400
categories: [Artificial Intelligence, Object Detection, YOLO, Training]
tags: [YOLO, Object Detection, Deep Learning, Anchor Boxes, Network Architecture]
thumbnail: assets/img/blog/YOLO_timeline_2023.PNG
---

The YOLO framework has undergone several iterations since its initial release in 2015 by Joseph Redmon and a team of collaborators (https://arxiv.org/pdf/1506.02640.pdf). It revolutionized real-time object detection capabilities. Redmon and Ali Farhadi subsequently developed YOLO V2 in 2016 (https://arxiv.org/pdf/1612.08242.pdf) and YOLO V3 in 2018 (https://arxiv.org/pdf/1804.02767.pdf), introducing advancements such as anchor boxes, the Darknet-19 architecture, and fully convolutional predictions in V2, and the Darknet-53 architecture and multi-scale predictions in V3.

{% include figure.liquid loading="eager" path="assets/img/blog/YOLO_timeline_2023.png" class="img-fluid rounded z-depth-1" %}

In 2020, Redmon announced his discontinuation of computer vision research due to concerns about military applications. Subsequently, other teams took over the development of the YOLO framework, resulting in more accessible articles. Alexey Bochkovskiy et al. published the V4 paper in 2020 (https://arxiv.org/pdf/2004.10934.pdf), focusing on optimizing network hyperparameters and introducing an IOU-based loss function. Soon after, Ultralytics entered the scene with YOLOv5, which featured an improved algorithm for anchor finding (https://github.com/ultralytics/yolov5). Ultralytics had previously implemented their own version of YOLO V3. The same team behind V4 published YOLOR in 2021 (https://arxiv.org/pdf/2105.04206.pdf), emphasizing multi-task learning for classification, detection, and pose estimation. Later in 2021, Megvii Technology developed YOLOX, reintroducing an anchor-free process (https://arxiv.org/pdf/2107.08430.pdf).

Interestingly, V7 was released in 2022 before V6 by the team responsible for V4. V7 focused on small optimizations, while V6, introduced by Meituan in 2022 (https://arxiv.org/pdf/2209.02976.pdf), emphasized model compression strategies such as quantization and distillation. Alibaba developed DAMO-YOLO later that year using neural architecture search (https://arxiv.org/pdf/2211.15444.pdf). Ultralytics improved upon the framework with the release of YOLOv8 earlier this year (https://github.com/ultralytics/ultralytics).

Meanwhile other teams have also created models labeled as “YOLO,” the discussion on other YOLO models and further details can be accessed in: (https://arxiv.org/pdf/2304.00501.pdf).

In summary, the YOLO framework has evolved through multiple iterations, addressing limitations and enhancing performance. This blog provides a very brief timeline of the development from original YOLO v1 to the latest YOLO v8, highlighting the key innovations, differences, and improvements made. Each iteration of the YOLO framework has brought various enhancements, ranging from network design to input resolution scaling.