# Vision-Detection
2D/3D vision detection algorithm

《目标检测前言》
one-stage：SSD、YOLO
two-stage：Faster-RCNN
1、two-stage 检测更准确
1）通过**专门模块去生成候选框（RPN**），寻找前景以及调整边界框（基于anchors）
生成候选框的过程当中呢，只是将感兴趣的目标前景进行寻找并框选出来，并未对其进行分类。
2）**基于之前生成的候选框**进行**进一步分类以及调整边界框（基于proposals）**
2、one-stage 检测速度快
基于anchors直接进行分类以及调整边界框；