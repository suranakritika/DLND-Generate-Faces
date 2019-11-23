# DLND-Generate-Faces
### Introduction
In this project, you'll use generative adversarial networks to generate new images of faces.

### Getting the project files
The project files can be found in our [public GitHub repo](https://github.com/udacity/deep-learning/tree/master/), in the face_generation folder. You can download the files from there, but it's better to clone the repository to your computer

This way you can stay up to date with any changes we make by pulling the changes to your local repository with git pull.

### Project Description
This project, will use Generative Adversarial Network to generate celebrity faces. Here, we are using GAN’s to build the model. The idea behind GANs is that you have two networks, a generator G and a discriminator D, competing against each other. The generator makes fake data to pass to the discriminator. The discriminator also sees real data and predicts if the data it's received is real or fake. The generator is trained to fool the discriminator, it wants to output data that looks as close as possible to real data. And the discriminator is trained to figure out which data is real and which is fake. What ends up happening is that the generator learns to make data that is indistiguishable from real data to the discriminator. The first layer is a fully connected layer which is reshaped into a deep and narrow layer, Then we use batch normalization and a leaky ReLU activation. Next is a transposed convolution where typically you'd halve the depth and double the width and height of the previous layer. Again, we use batch normalization and leaky ReLU. For each of these layers, the general scheme is convolution > batch norm > leaky ReLU.
