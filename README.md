# Image Captioning using VGG16 Feature Extraction and LSTM Decoder

### **Introduction**

This project focuses on building an image captioning model using the Flickr8k dataset, which consists of 8,000 images, each paired with five captions. The dataset contains images and a separate captions file, which links images to their corresponding descriptions. The objective is to generate descriptive captions for images using deep learning techniques, particularly leveraging the VGG16 pretrained model for feature extraction and an LSTM (Long Short-Term Memory) network for sequence generation.

#### **Model Architecture**

The model consists of two parts:

1. ***Image Feature Layer***: This layer processes the features extracted from the images using the VGG16 model. It includes a dense layer with dropout for regularization.

2. ***Caption Generation Layer***: This layer processes the tokenized caption sequences with an LSTM layer to capture the temporal dependencies between words in the caption.

The two parts are merged, and a final dense layer with a softmax activation function is used to generate the predicted words in the caption.
