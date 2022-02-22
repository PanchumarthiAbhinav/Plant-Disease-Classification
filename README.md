# Plant-Disease-Classification
## Classification of plant diseases using Convolutional neural networks

* The model is built based on Teacher-Student Architecture, Which consists of three classifier Teacher, Decoder and Student Classifier
* Teacher and Student classifiers use VGG-16 Architecture which are loaded with the weights of the model trained on Image Net Dataset(Which is known as Transfer Learning).
* Using transfer learning decreases the computational complexity and also increases the accuracy
* The dataset used is publicly available [Plant Village Dataset](https://www.kaggle.com/abdallahalidev/plantvillage-dataset)
* The above model provides a better visual view of the infected parts of plants, Which can be seen in the below image

![Visual View](https://github.com/PanchumarthiAbhinav/Plant-Disease-Classification/blob/main/img/Visual%20view.jpg)
* The output from the Teacher classifier is used as input for the decode classifier whose output is the visual view shown above, Later this image is used as input for the student classifier for training.
![Teacher Student Model](https://github.com/PanchumarthiAbhinav/Plant-Disease-Classification/blob/main/img/Teacher%20Student%20Model.jpg)

* The above `.ipynb` file contains the code upto the model building, training and saving
* We have used the `accuracy` metric for measuring the model
* The loss function used is `Categorical Cross-Entropy Loss` which is used for tasks where we are classifying more than two categories else `Binary Cross-Entropy Loss` can be used.
* You could check out the code in the file [Plant Disease Classification](https://github.com/PanchumarthiAbhinav/Plant-Disease-Classification/blob/main/Plant%20Disease%20Classification.ipynb)


![Reference](https://arxiv.org/pdf/1905.13523v2.pdf)

