# Style-Transfer-Learning-CNN
**Neural Style Transfer**
An 'artistic' application of Convolutional Neural Networks called **image style transfer**.
Style transfer is an application of **transfer learning** where you have a 'content image' and a 'style image' and the objective is to transfer the style from the style image to the content image**.**
**The training task is to learn the candidate image**. That is, during training, the individual pixel values of the candidate image are learnt. You randomly initialize the candidate image and then update the pixels using backpropagation.

For transfer learning, a pre-trained model, VGGNet is being used, and its last fully connected layer is removed since our task is not to classify the image. Here, we use the pre-trained weights of the model to update the candidate image instead of updating the model weights. Since there are no prebuilt functions to train these type of networks in Keras, we have used custom functions.
