# cnn-fashion_image_classification
Fashion Image Classification Experiment based on CNN, Analysis on Different Parameters using Tensorflow

Final Project GE2324 Art and Science of Data - Grade: 90/100
> Leturer: Dr. MA Chen
> City University of Hong Kong

Reference of dataset:
>Param Aggarwal. 2019. Fashion Product Images Dataset. www.kaggle.com. Retrieved April 15, 2022
from https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset

## Model Architectures
![model_table](/images/model_table.png "model_table")

Parameters tested: Different Dropout values and Different Optimizer

## Results
Model 1
![model1](/images/model1.png "model1")

Model 2
![model2](/images/model2.png "model2")

Model 3
![model3](/images/model3.png "model3")

Model 4
![model4](/images/model4.png "model4")

## Discussions
Dropout:
> As dropout is used to improve the model's generalization, higher dropout in the first hidden layers after
the convolutional layers could improve the model performance due to more output randomly set to 0. This
affects the weight updating process of backpropagation, resulting in a better model when used to test
images that were not inputted as training data [5].

Optimizer:
> The adam optimizer models are
better with a 0.01-0.02 difference than the RMSProp models.
Since Adam optimizers were built inheriting the features of RMSProp and another optimizer called
Adagrad, Adam uses the second moment of the gradients as well, as opposed to the adapting learning rate
based on the first moment in RMSProp. Additionally, the learning rate must be manually configured for
several uses with RMSProp, and the suggested value does not fit every case [3]. Therefore, Adam's higher
accuracy could be attributed to a feature that allows the learning rate to be modified for each network
weight independently

Further details attached on the paper
> Report_Fashion Image Classification.pdf
