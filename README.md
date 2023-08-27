# Image-generation-using-DCGAN using custom training process

DCGAN is a notable contribution that introduced deep convolutional networks into GANs. It's a specific architecture that employs convolutional layers in both the generator and discriminator. DCGAN demonstrated that the architectural design plays a crucial role in stabilizing the GAN training process and generating high-quality images.

Research Paper refered : https://arxiv.org/pdf/1511.06434

For more similar papers, refer here: https://github.com/joshir199/Revisiting-famous-Deep-Learning-research-papers

-------------------------------------------
Architecture guidelines for stable Deep Convolutional GANs from above paper:

• Replace any pooling layers with strided convolutions (discriminator) and fractional-strided convolutions (generator).

• Use batchnorm in both the generator and the discriminator.

• Remove fully connected hidden layers for deeper architectures.

• Use ReLU activation in generator for all layers except for the output, which uses Tanh.

• Use LeakyReLU activation in the discriminator for all layers.


-----------------------------------------------
Dataset used for this DC-GAN model training :

Description: Fashion-MNIST is a dataset of Zalando's article images consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes.

Dataset source: https://www.tensorflow.org/datasets/catalog/fashion_mnist
*********************

![](https://github.com/joshir199/Image-generation-using-DCGAN/blob/main/dc_gan_generated_image.gif)

->  Training result showing how generator learns to generate better images


******************
# Generator Model architecture

![](https://github.com/joshir199/Image-generation-using-DCGAN/blob/main/model/model%20summary/generator.png)


******************
# Discriminator Model Architecture

![](https://github.com/joshir199/Image-generation-using-DCGAN/blob/main/model/model%20summary/discriminator.png)

*****************
# Deep Convolutional GAN model architecture

![](https://github.com/joshir199/Image-generation-using-DCGAN/blob/main/model/model%20summary/GAN_model_summary.png)
***********************

# Training Loss graph:

![](https://github.com/joshir199/Image-generation-using-DCGAN/blob/main/DC-GAN_training_loss_graph.png)

