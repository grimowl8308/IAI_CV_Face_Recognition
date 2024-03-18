"
# IndonesiaAI_ComputerVision

### Introduction
- Face recognition technology, enabled by artificial intelligence (AI), has become increasingly prevalent across various industries. 
- This technology involves analyzing facial features to identify and verify individuals. 
- AI algorithms, particularly *convolutional neural networks (CNNs)*, extract unique features from facial images, encode them into numerical representations, and match them to known individuals. 
- Face recognition technology offers benefits such as enhanced security, improved efficiency, and personalized experiences. 
- However, it also raises ethical and privacy concerns.


### Getting Started
This project was entirely conducted on Kaggle. Here are the steps to run it from your computer:
1. Download all files in this repository (`.ipynb` and `.zip`) to your working directory.
2. Create a new directory `./input` in your working directory and extract the `celeba-subset.zip` file into it.
3. You can now run the notebook on your computer, but it is recommended to use GPU to speed up the training process.


### The Result
Broadly, every notebook consists of three main sections:

1. **Preprocess**: Prepares data from `./input` through data clean-up and grouping, resulting in ready-to-use data in `./train`, `./val`, and `./test`.
2. **Transfer Learning**: A *CNN model* is chosen (according to the notebook name) to undergo the *transfer learning* process, including training some base layers, constructing *fully-connected layers*, applying *callback* strategies, and *hyperparameter tuning* to achieve optimal results.
3. **Testing**: The model is tested on test data, obtaining a series of classification metrics and other metrics. The model is also tasked with making predictions on images from the internet.

<br>Here are the performance results of transfer learning from each optimized model.

|               | InceptionV3 |  VGG16 | ResNet101 | ResNet152 |
|---------------|-------------|--------|-----------|-----------|
| Accuracy      |    97.60    |  96.39 |   91.98   |   95.79   |
| Precision     |    96.15    |  95.59 |   91.00   |   96.92   |
| Recall        |    98.04    |  95.59 |   89.22   |   92.65   |
| F1            |    97.09    |  95.59 |   90.10   |   94.74   |
| Loss          |    17.12    |  10.21 |   16.16   |   11.25   |
| Inference (s) |    12.10    |   7.77 |   12.86   |   18.24   |
" 
