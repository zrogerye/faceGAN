# Generative Adversarial Network Generated Faces
Contains the JupyterNotebook I used to train models, the resulting images of 25 epoch generations of training, and the models themselves.

The dataset used to train models: https://www.kaggle.com/ashwingupta3012/human-faces

# Compilation of Trained Images
https://user-images.githubusercontent.com/67408272/128583488-0f54b8d2-ac86-4352-8811-63b913144e3f.mp4

# Notes
25 Generations of training is definitely not enough to claim substantial outcomes, though, the results contain features that bear some resemblance to a final product of human faces. We generate a batch of images using the generaton and pass them to the discriminator. Loss is calculated by setting the target labels to 1 (real) since the generator's objective is to "fool" the discriminator. The objective of the discriminator is to differentiate between our products to original images. We use the loss to perform gradient descent (changing the weights of the generator to generate realistic images) to better "fool" the discriminator.
![losses](https://user-images.githubusercontent.com/67408272/128583919-4677b013-c04a-41f7-a219-7bc1e7ec6e14.png)
![scores](https://user-images.githubusercontent.com/67408272/128583921-fa740d41-2002-4cbf-9f3e-0a3c51de38c5.png)

