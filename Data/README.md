# Augmented Images

![result](https://github.com/ParthMehta15/Fire-and-Gun-Anomaly-Detection/blob/main/images/fire_gun.jpg "Model Output")



### Weights File Backup

YOLOv3 pretrained weights - Download [Weights](https://pjreddie.com/media/files/yolov3.weights) 

Pre-trainned Weights for convolution layers - Download [Conv_weights](https://pjreddie.com/media/files/darknet53.conv.74)


[Dataset](https://www.kaggle.com/parthmehta15/gunfire-yolo)

Training done on google collab - [Jupyter notebook](https://colab.research.google.com/drive/1rtBmGPgYQGwpAPkcqqgb_RE6fZj89ceb?usp=sharing)

Demo: [Video](https://www.linkedin.com/posts/parthmehta15_deeplearning-neuralnetworks-ai-activity-6725707478996160512-ixJp)

### Paper
[Fire and Gun Violence based Anomaly Detection System Using Deep Neural Networks](https://ieeexplore.ieee.org/document/9155625) <br>
Proceedings of the [International conference on Electronics and Sustainable Communication Systems - ICESCS 2020](https://ieeexplore.ieee.org/servlet/opac?punumber=9145513) <br>
ISBN: 978-1-7281-4107-7 <br>
978-1-7281-4108-4/20/©2020 IEEE <br>




The following augmentations were used:
• Random zoom (between 1.3x to 1.5x)
• Random skew.
• Random distortions with a 4x4 window.
• Random crops containing 80-90% of the image
• Random combinations of all these four augmentations

To train the network, the data is prepared as follows:
• The training data will have positive as well as negative examples.
• For the positive pairs, each coloured database image (real face) is paired with the 6 augmented sketch images in addition to the original sketch image, making total of seven positive (database image, sketch image) pairs.
• For the negative pairs, each colour database image (real face) of a person is paired with randomly sampled sketch images of a different person. To keep the positive and negative classes balanced, a total of seven such pairs are created.
