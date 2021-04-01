# Hybrid Deep Learning Model for Stock Price Prediction

## Stock price prediction  
- Challenging task 
- Highly dynamic nature (highly random movement)

## stock price prediction by hybride model of LSTM and GRU
This is the stock price prediction model created on the basis of the research paper [hossain2018.pdf](https://github.com/sourabhsingh282/stockprice_prediction_LSTM_GRU/files/6244153/hossain2018.pdf)

## I have trained this Model on Local computer containing following specification
- CPU AMD ryzen4800H Processor 8 core 16 thread CPU and 
- GPU Nvidia 1650Ti
## Deep Neural Network (DNN)
- An advanced branch of ANN. 
- DNN has gained enormous popularity due to its effectiveness on prediction based problems. 
- DNN has been showing promising performance for problems such as speech recognition, natural language processing, computer vision, robotics, computational finance.
- 
# LSTM Unit

- Derivative of Recurrent Neural Network (RNN), which operates on sequential data. 
- It has a memory unit that can keep track of the certain amount of training data (to solve the long term dependencies problem).
- Can learn automatically when to forget the memory for a particular sequence.
 
 # GRU
- Main difference between LSTM and GRU - GRU combines the forget and the input gates into a single update gate.
- Also merges the cell state and the hidden state and makes some other changes
- Simpler yet faster network than the standard LSTM models.
- Basic purpose is similar to LSTM.


#  Hybrid Network
- Combination of LSTM and GRU.
- Proposed Model :
- First, we pass the input vector to the LSTM unit with one hidden layer and we get the output Flstm . 
- Next, we pass Flstm to as the input of GRU unit. At the second layer we get the Fgru as the output of GRU unit. 
- Then, we pass Fgru into dense network followed by a linear activation. 
- Finally, we calculate Euclidean loss (L2 loss), between the prediction and the ground truth and back propagate this loss to the network to update the model parameters. After 20 epochs by demonstrating loss curve we get our trained model.



 
