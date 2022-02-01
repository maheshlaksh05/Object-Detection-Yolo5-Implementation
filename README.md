# Object-Detection-Yolo5-Implementation
Yolo5 Object Detection 
What is YOLOv5?
i) History and Controversy
YOLO stands for You Look Only Once and it is one of the finest family of object detection models with state-of-the-art performances.

Its first model was released in 2016 by Joseph Redmon who went on to publish YOLOv2 (2017) and YOLOv3 (2018). In 2020 Joseph Redmon stepped out from the project citing ethical issues in the computer vision field and his work was further improved by Alexey Bochkovskiy who produced YOLOv4 in 2020.

YOLOv5 is the next controversial member of the YOLO family released in 2020 by the company Ultranytics just a few days after YOLOv4.

ii) Where is YOLOv5 Paper?

YOLOv5 is controversial due to the fact that no paper has been published yet (till the time of writing this) by its author Glenn Jocher for the community to peer review its benchmark. Neither it is seen to have implemented any novel techniques to claim itself as the next version of YOLO. Instead, it is considered as the PyTorch extension of YOLOv3 and a marketing strategy by Ultranytics to ride on the popularity of the YOLO family of object detection models.

But one should note that when YOLOv3 was created, Glenn Jocher (creator of YOLOv5) contributed to it by providing the implementation of mosaic data augmentation and genetic algorithm.

iii) Is YOLOv5 Good or Bad?
Certainly, the controversy behind YOLOv5 is just due to its choice of name, but it does not take away the fact that this is after all a great YOLO object detection model ported on PyTorch.

Probably if you are just a developer, you would not even care about the controversy and may enjoy working with YOLOv5 due to its ease of use. (As we will see in the examples of this tutorial)

YOLOv5 Architecture
![image](https://user-images.githubusercontent.com/97341259/151928072-89fada60-2f48-43a0-bb17-02b4f0714fd6.png)

YOLOv5 Architecture
(Source)
![image](https://user-images.githubusercontent.com/97341259/151928103-9bbcca05-3f2a-4563-b6eb-aad898c822f7.png)

The YOLO family of models consists of three main architectural blocks i) Backbone, ii) Neck and iii) Head.

YOLOv5 Backbone: It employs CSPDarknet as the backbone for feature extraction from images consisting of cross-stage partial networks.
YOLOv5 Neck: It uses PANet to generate a feature pyramids network to perform aggregation on the features and pass it to Head for prediction.
YOLOv5 Head:  Layers that generate predictions from the anchor boxes for object detection.
Apart from this YOLOv5 uses the below choices for training –

Activation and Optimization: YOLOv5 uses leaky ReLU and sigmoid activation, and SGD and ADAM as optimizer options.
Loss Function: It uses Binary cross-entropy with logits loss.
Different Types of YOLOv5
What is YOLOv5
YOLOv5 Model Comparison
![image](https://user-images.githubusercontent.com/97341259/151928188-1d40e8fd-8e18-4322-8513-4f9e929540cf.png)

YOLOv5 has multiple varieties of pre-trained models as we can see above. The difference between them is the trade-off between the size of the model and inference time. The lightweight model version YOLOv5s is just 14MB but not very accurate. On the other side of the spectrum, we have YOLOv5x whose size is  168MB but is the most accurate version of its family.


Comparison Graph
Comparison Graph
