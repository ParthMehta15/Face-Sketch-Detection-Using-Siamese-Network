### Augmented Images

![result](https://github.com/ParthMehta15/Face-Sketch-Detection-Using-Siamese-Network/blob/main/images/augmented.png "Augmented")



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
