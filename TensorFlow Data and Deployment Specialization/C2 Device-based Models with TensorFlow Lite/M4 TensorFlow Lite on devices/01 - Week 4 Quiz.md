# Week 4 Quiz
## Latest Submission Grade: 100%

## Question 1
Which Devices support TensorFlow Lite for Inference? (Check all that apply)
* RISC
* **Coral**
> Correct
* **Raspberry Pi**
> Correct
* **Sparkfun Edge**
> Correct

## Question 2
With a Raspberry Pi, how can you use TensorFlow?
* Training Only
* Inference Only
* **Inference and Training**
* It doesn’t work on Pi
> Correct

## Question 3
If you only want to do inference on a Pi, what’s the best way?
* Do nothing, the Pi base image has TensorFlow in it
* Compile all of TensorFlow from Source and run it
* **Install the standalone interpreter using pip**
* Install the full TensorFlow with Pip install
> Correct

## Question 4
When using ImageNet on a Raspberry Pi for Image Classification, how many classes are supported?
* 100
* **1000**
* 800
* 500
> Correct

## Question 5
How do you initialize the standalone interpreter in Python?
* tf.lite.load(lite_model)
* tf.lite.load(saved_model)
* tf.lite.Interpreter(directory_of_saved_model)
* **tf.lite.Interpreter(directory_of_lite_Model)**
> Correct

## Question 6
How do you get the input tensors for a model with the standalone interpreter?
* Call get_input_details() after initializing the interpreter
* **Call get_input_details() after calling allocate_tensors() on the interpreter*
* Call get_input_tensors() after initializing the interpreter
* Call get_input_tensors() after calling allocate_tensors() on the interpreter
> Correct

## Question 7
How do you perform inference using the interpreter?
* **Set the Input tensor with the set_tensor command and then call invoke()**
* Just call invoke(), TensorFlow can do the rest
* Call invoke(), and pass it the input tensor
* Call invoke(), and pass it both the input and output tensors
> Correct

## Question 8
How do you read the results of inference using the interpreter?
* Call invoke(), pass it the input and output tensors, and then read the output tensor
* Call invoke(), pass it the input tensor, read the results
* **Call invoke(), and then call get_tensor() on the interpreter to read the output**
* Call invoke(), and the the output will be rendered automatically
> Correct
