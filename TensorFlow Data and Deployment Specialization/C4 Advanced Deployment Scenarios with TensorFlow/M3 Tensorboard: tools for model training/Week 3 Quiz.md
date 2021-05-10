# Week 3 Quiz
## Latest Submission Grade: 100%

## Question 1
If you want to track training data, such as accuracy and loss and visualize it on TensorBoard, what programming pattern would you use?
* Store them in a database and point TensorBoard at that DB
* **Store them in a log file and use epoch-by-epoch callbacks to update it. Have Tensorboard read that log file**
* It just happens automatically
* Store them in a log file, and at the end of the training, pass that to TensorBoard
> Correct

## Question 2
If you are using a callback to manage logging of data for TensorBoard, where would you specify it?
* After you’re done training
* **During the model.fit process**
* When you design the model
* While preprocessing the data
> Correct

## Question 3
What’s the name of the class in TensorFlow that handles and manages logging to TensorBoard?
* tf.keras.TensorBoard.callbacks
* tf.logs.TensorBoard.callback
* tf.TensorBoard.callback
* **tf.keras.callbacks.TensorBoard**
> Correct

## Question 4
How do you get a histogram plotting each epoch in your training?
* Set use_histogram=true and histogram_freq=1
* **Set histogram_freq=1**
* Set histogram_freq=all
* Set use_histogram=true
> Correct

## Question 5
If you want to upload your logs to tensorboard.dev to share with others, what command do you use?
* tensorboard upload dev --logdir ./logs
* **tensorboard dev upload --logdir ./logs**
* tensorboard dev --logdir ./logs
* tensorboard upload --logdir ./logs
> Correct

## Question 6
When you share your logs on tensorboard.dev, what is the URL signature that you share with others?
* tensorboard.dev/[code]
* tensorboard.dev/logs/[code]
* tensorboard.dev/board/[code]
* **tensorboard.dev/experiment/[code]**
> Correct

## Question 7
If you want to write an image to logs for TensorBoard to represent it, what API call should you use?
* tf.summary() - with image as a parameter
* image.write(tf.summary.TensorBoard)
* **tf.summary.image() -- with image as a parameter**
* tf.summary.write_image() - with image as a parameter
> Correct

## Question 8
If you have written logs (including images and more) to logs/train_data, and want to inspect them with TensorBoard, what’s the command to use?
* %tensorboard --dir logs/train_data
* %tensorboard --logs logs/train_data
* **%tensorboard --logdir logs/train_data**
* %tensorboard --logdir train_data
> Correct

## Question 9
If you want to create a simple, custom, callback on-the-fly, what API would you use?
* tf.keras.callbacks.Dynamic
* **tf.keras.callbacks.LambdaCallback**
* tf.keras.callbacks.Lambda
* tf.keras.callbacks.Simple
> Correct

## Question 10
Which module in TensorFlow provides APIs to store data that TensorBoard and other tools can use?
* **tf.summary**
* tf.debug
* tf.data
* tf.logs
> Correct
