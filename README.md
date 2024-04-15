# student loans with deep learning

Data Source: https://static.bc-edx.com/mbc/ai/m6/datasets/student_loans.csv

The goal is create a neural network to predict the credit ranking of a person using the provided features from the data source 

The neural network goes as followed
number_input_features = 11

hidden_nodes_layer1 = 6

hidden_nodes_layer2 = 3

out_layer = 1

nn = Sequential()

nn.add(Dense(units=hidden_nodes_layer1, input_dim=number_input_features, activation="relu"))

nn.add(Dense(units=hidden_nodes_layer2, activation="relu"))

nn.add(Dense(units=out_layer, activation="linear"))

The summary goes as followed

Model: "sequential_5"

 Layer (type) ------------------------ Output Shape -------------------------- Param #
 
 dense_15 (Dense)---------------------- (None, 6)------------------------------- 72        
                                                                 
 dense_16 (Dense)---------------------- (None, 3)------------------------------- 21        
                                                                 
 dense_17 (Dense)---------------------- (None, 1)-------------------------------  4         
                                                                 
=================================================================
Total params: 97
Trainable params: 97
Non-trainable params: 0

We then compile the model and fit said model.
After which we measure the model's loss and accuracy metrics

The scores goes as followed 

13/13 - 1s - loss: 0.6881 - mse: 0.6881 - 526ms/epoch - 40ms/step

Loss: 0.6880970001220703, Accuracy: 0.6880970001220703

As we can see the data doesn't actually perform as well as we hoped
As shown in the graphic 

![Untitled](https://github.com/msills30/student_loans_with_deep_learning/assets/127795370/ffeca48e-6407-4109-bbc3-071e84c19652)


