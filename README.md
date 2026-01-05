### Sign2Word
The Sign2Word model addresses the more complex task of word recognition through a hierarchical classification approach. It simultaneously predicts broad categories (super-classes) and specific words (fine-classes) by sharing learned features between two output branches. This model utilizes convolutional and dense layers arranged in a multi-output architecture, implemented with TensorFlow’s functional API for flexibility. The training process balances the two losses with weighted loss functions and employs similar optimization and regularization techniques as the letter model.

Real-time detection is a key part of the Sign2Text system, where the model process live video frames to predict words instantly. Efficient model design and preprocessing minimize delay, allowing smooth interaction.

#### Datasets used:
**[Sign2Word](https://www.kaggle.com/datasets/risangbaskoro/wlasl-processed)**
