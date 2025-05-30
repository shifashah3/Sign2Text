## Sign2Text 
The Sign2Text project consists of two deep learning models developed using TensorFlow and Keras, which are powerful libraries for building and training neural networks.

### Sign2Letter
he Sign2Letter model is a convolutional neural network (CNN) designed to classify individual letters from grayscale images of hand signs. It uses multiple convolutional layers combined with batch normalization and dropout to extract robust spatial features while preventing overfitting. The model is compiled with the Adam optimizer and trained using categorical crossentropy loss, with callbacks like EarlyStopping and ReduceLROnPlateau to dynamically adjust learning rates and avoid unnecessary training.

### Sign2Word
The Sign2Word model addresses the more complex task of word recognition through a hierarchical classification approach. It simultaneously predicts broad categories (super-classes) and specific words (fine-classes) by sharing learned features between two output branches. This model utilizes convolutional and dense layers arranged in a multi-output architecture, implemented with TensorFlow’s functional API for flexibility. The training process balances the two losses with weighted loss functions and employs similar optimization and regularization techniques as the letter model.

Real-time detection is a key part of the Sign2Text system, where the models process live video frames to predict letters or words instantly. Efficient model design and preprocessing minimize delay, allowing smooth interaction.

#### Datasets used:
**[Sign2Letter](https://www.kaggle.com/datasets/grassknoted/asl-alphabet)**
**[Sign2Word](https://www.kaggle.com/datasets/risangbaskoro/wlasl-processed)**
