# GAN-model

Generative Adversarial Neural Network:
  GANs are mainly used for synthetic data generation like images and with an advanced model we could perform super-resolution, smoke removal and etc., There are also conditional GANs which would also us to have control over what data to be generated. 
  
This code is a basic GAN model which is built over the fashion mnist dataset which is loaded from TensorFlow datasets. The following methods have been enhanced to build this GAN:

                                1.	Set up the environment
                                2.	Build Data Pipeline
                                3.	Create a Generator and Discriminator
                                4.	Build a custom training loop
                                5.	Generate new images
                                
Initially, we load the fashion_mnist dataset then we build a generator and discriminator where the generator produces images that are fake and the discriminator has to identify which is fake and which is original.0 represents a true image whereas 1 represents a fake image. The key thing here is to maintain the balance between the discriminator and generator hence we built a custom training loop. Through this, we maintain the balance by rewarding our discriminator if it correctly identifies fake images and rewarding the generator if it fools the discriminator.


The final model has been trained over 500 epochs in order to produce accurate images



