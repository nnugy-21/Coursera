# Week 3 Quiz
## Latest Submission Grade: 100%

## Question 1
If X is the standard notation for the input to an RNN, what are the standard notations for the outputs?
* Y
* H
* **Y(hat) and H**
* H(hat) and Y
> Correct

## Question 2
What is a sequence to vector if an RNN has 30 cells numbered 0 to 29
* **The Y(hat) for the last cell**
* The total Y(hat) for all cells
* The average Y(hat) for all 30 cells
* The Y(hat) for the first cell
> Correct

## Question 3
What does a Lambda layer in a neural network do?
* Pauses training without a callback
* There are no Lambda layers in a neural network
* **Allows you to execute arbitrary code while training**
* Changes the shape of the input or output data
> Correct

## Question 4
What does the axis parameter of tf.expand_dims do?
* Defines the dimension index to remove when you expand the tensor
* Defines if the tensor is X or Y
* **Defines the dimension index at which you will expand the shape of the tensor**
* Defines the axis around which to expand the dimensions
> Correct

## Question 5
A new loss function was introduced in this module, named after a famous statistician. What is it called?
* **Huber loss**
* Hubble loss
* Hawking loss
* Hyatt loss
> Correct

## Question 6
What’s the primary difference between a simple RNN and an LSTM
* LSTMs have a single output, RNNs have multiple
* **In addition to the H output, LSTMs have a cell state that runs across all cells**
* LSTMs have multiple outputs, RNNs have a single one
* In addition to the H output, RNNs have a cell state that runs across all cells 
> Correct

## Question 7
If you want to clear out all temporary variables that tensorflow might have from previous sessions, what code do you run?
* tf.keras.clear_session
* tf.cache.clear_session()
* **tf.keras.backend.clear_session()**
* tf.cache.backend.clear_session()
> Correct

## Question 8
What happens if you define a neural network with these two layers? <br>
tf.keras.layers.Bidirectional(tf.keras.layers.LSTM(32)), <br> <br>
tf.keras.layers.Bidirectional(tf.keras.layers.LSTM(32)), <br> <br>
tf.keras.layers.Dense(1),
* Your model will compile and run correctly
* Your model will fail because you have the same number of cells in each LSTM
* **Your model will fail because you need return_sequences=True after the first LSTM layer**
* Your model will fail because you need return_sequences=True after each LSTM layer
> Correct
