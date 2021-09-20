Since the data is very less (25 faces), the first step is augment images of the dataset. The following augmentations were used:
• Random zoom (between 1.3x to 1.5x)
• Random skew.
• Random distortions with a 4x4 window.
• Random crops containing 80-90% of the image
• Random combinations of all these four augmentations
2. Augmentation increases the size of the dataset and reduces the risk of model overfitting.
3. The proposed network is a Siamese Network which means it has two inputs. One input is for the real image (database image), and the other input is for the sketch image which we want to search in the database.
4. To train the network, the data is prepared as follows:
• The training data will have positive as well as negative examples.
• For the positive pairs, each coloured database image (real face) is paired with the 6 augmented sketch images in addition to the original sketch image, making total of seven positive (database image, sketch image) pairs.
• For the negative pairs, each colour database image (real face) of a person is paired with randomly sampled sketch images of a different person. To keep the positive and negative classes balanced, a total of seven such pairs are created.
• This means we end up with 14 training pairs per person in the database (seven positive pairs, and seven negative pairs), as shown in Figure 1.
• We assign the positive pairs a label of ‘1’ and the negative pairs a label of ‘0’.
• The prepared data is shuffled randomly and 20% of the data is held out for testing purposes.
