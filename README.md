# Image Classification for cats and dogs

Innitial dataset was lowered from cca 30.000 images to 2000 and the number of epochs was lowered from 25 to 3, as even with numbers so low it takes my laptop 5h to train the model.

The end result is thus pretty horrible as it classifies everything as cca 50.6% dog and 49.4% cat, 
but with should I have a GPU available and could train it properly I would only need to re-add the rest of the images and increase the number of epochs (though not above 50 as it would result in overfitting).

#### Summary
I documented everything I found important in the jupyter notebook file with markdown, step by step as I added it in **main.ipynb** file.

But the Keras model used here is a convolutional neural network designed for image classification.
The model consists of multiple layers, including rescaling, separable convolution, batch normalization, and global average pooling. 
It follows a deep learning architecture with residual connections to enhance feature reuse and learning. The network utilizes dropout for regularization to prevent overfitting during training. The final layer is a dense layer with an activation function tailored for binary classification, 
as the task involves categorizing images into two classes: cats or dogs. This Keras model is well-suited for image recognition tasks and is trained using the Adam optimizer with a binary cross-entropy loss function.
