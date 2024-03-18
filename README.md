What is Feed Forward Network
==
Feedforward neural networks are a fundamental architecture in artificial neural networks. In a feedforward network, information travels unidirectionally from the input layer through one or more hidden layers to the output layer. Feedforward networks are versatile, used for tasks like classification and regression, and serve as the basis for more advanced neural network architectures

<img width="705" alt="Screen Shot 2024-03-16 at 3 18 29 PM" src="https://github.com/noderdev/Feed-Forward-Network-for-Binary-Image-Classification/assets/29915581/e5d1d8dd-3c16-49ba-a043-346822c36fef">

Problem Statement
==
This problem consists of classifying images as food and non-food images. We will build a feed forward network to classify the images by training our classifier on the training data set provided and tune our model’s hyperparameters by evaluating the model on the validation data set. We will tune the model’s architecture parameters like the number of layers, neurons per layer by considering various possible architectures. We will also introduce different regularizations and tune the hyperparameters associated with each regularization. Finally, we will evaluate the selected model on the test dataset provided.

Requirements
==
``` Make sure to have tensorflow 2.0 >= installed. Install sklearn, numpy , matplotlib ```

Dataset
==
The dataset consists of food and non-food images for binary classification. To get the dataset, download from the link below:-
```
https://drive.google.com/file/d/1ee6ga_Ch2luZFRKHnC1xjferdnzLFEMH/view?usp=sharing
```

Results
==
Comparison of the base model's performance (without regularization) with different regularization techniques :-

<img width="501" alt="Screen Shot 2024-03-16 at 3 20 01 PM" src="https://github.com/noderdev/Feed-Forward-Network-for-Binary-Image-Classification/assets/29915581/a4f1058c-14f1-459c-98d2-dae7a27f1cc4">

The model with 3 hidden layers having 128 neurons in first layer, 32 neurons in second and 8 neurons in second layer with early with L2 regularization of 0.1 is giving an accuracy of 81% on test and an f1 score of 0.81 as well. Dropout regularization is also giving similar results. Hence, we can use either of the regularization techniques with our base model
