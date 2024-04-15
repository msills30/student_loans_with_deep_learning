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
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 dense_15 (Dense)            (None, 6)                 72        
                                                                 
 dense_16 (Dense)            (None, 3)                 21        
                                                                 
 dense_17 (Dense)            (None, 1)                 4         
                                                                 
=================================================================
Total params: 97
Trainable params: 97
Non-trainable params: 0


