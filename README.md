# Pneumonia-AI
A Deep Learning approach to classify lung X-rays to normal or Pneumonia affected lungs.

## Dataset
The data has been provided by kaggle to help automate the process of detecting diseases from medical images.
* Chest-X-Ray Images - https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia
* The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).
![Data Format](https://i.imgur.com/jZqpV51.png)

## Network Architecture
Clearly, it is an image classification problem. Hence, a custom CNN network has been used with the following architecture:-
* 3 (3 x 3) 2D Convolutional Layers with relu activation
* Each convolutional layer followed bya (2 x 2) 2D Max Pooling
* Two fully-connected layers with 50% dropout.

![architecture](https://user-images.githubusercontent.com/41809968/59549458-5cab7280-8f7b-11e9-8bed-5b7be5eeee35.png)

## Training
* The images are prprocessed and resized to (150 , 150).
* The model is compiled using Adam optimizer , binary crossentropy as loss and accuracy as metrics.
* The model is trained for 20 epochs.
* An accuracy of around 90% is achieved by the model on the test data set.

## To-do List
- [x] Build a model and train it
- [x] Evaluate the model
- [ ] Building a landing page using Flask
- [ ] Deploy the app
