Week 2 Quiz
## Latest Submission Grade: 100%

## Question 1
What is the correct syntax for the first layer in a convolutional neural network that takes an MNIST (28x28 monochrome) input? 
* **model.add(tf.layers.conv2d({inputShape: [28, 28, 1], kernelSize: 3, filters: 8, activation: 'relu'})); **
* model.add(tf.layers.conv({inputShape: (28, 28, 1), kernelSize: 3, filters: 8, activation: 'relu'}));
* model.add(tf.layers.conv2d({inputShape: [28, 28], kernelSize: 3, filters: 8, activation: 'relu'}));
* model.add(tf.layers.conv({inputShape: [28, 28, 1], kernelSize: 3, filters: 8, activation: 'relu'}));
> Correct

## Question 2
What is the correct syntax for adding a maxPooling2D layer to a Convolutional neural network in JavaScript?
* model.add(tf.layers.maxPooling2D({poolSize: [2, 2]}));
* model.add(tf.layers.maxPooling2D({poolSize =  [2, 2]}));
* **model.add(tf.layers.maxPooling2d({poolSize: [2, 2]}));**
* model.add(tf.layers.maxPooling2d({poolSize = [2, 2]}));
> Correct

## Question 3
What is the correct syntax for compiling a model with an optimizer, loss function and metrics? 
* model.compile({  tf.optimizer: tf.train.adam(), tf.loss: 'categoricalCrossentropy', tf.metrics: ['accuracy']});
* **model.compile({  optimizer: tf.train.adam(), loss: 'categoricalCrossentropy', metrics: ['accuracy']});**
* model.compile({  optimizer = tf.train.adam(), loss = 'categoricalCrossentropy', metrics = ['accuracy']});
* model.compile({  optimizer: tf.train.adam(); loss: 'categoricalCrossentropy'; metrics: ['accuracy']});
> Correct

## Question 4
How do you correctly pass a set of validation data called textXs and testYs to the model.fit method in JavaScript?
* **Use validationData: [testXs, testYs] in the list of parameters sent as the third parameter to model.fit**
* Use validationData: [testXs, testYs] in the list of parameters to model.fit
* Use validationData= [testXs, testYs] and pass it to the model.fit method
* Use validationData = [testXs, testYs] in the list of parameters to model.fit
> Correct

## Question 5
How do you get the built in callbacks visualizer with TensorFlow.js?
* **Include the tfjs-vis script, set a callback in model.fit, and set it to a const that called show.fitCallbacks() on the tfvis object**
* Include the tfjs-vis script and it will work automatically
* Include the tfjs-vis script, call show.fitCallbacks() on the tfvis object
* Include the tfjs-vis script, set a callback in model.fit and it will work automatically
> Correct

## Question 6
If you want to see loss, validation loss, accuracy and validation accuracy on each epoch while training, how do you do this? 
* Create a list containing text values [“loss=true”, “val_loss=true”, “acc=true”, “val_acc=true”] and pass it to fitCallbacks() as a parameter
* Create a list containing [1, 1, 1, 1] indicating that you want those 4 values to be true and pass it to the fitCallbacks() as a parameter
* Create a list setting loss=true, val_loss=true, acc=true, val_acc=true, and pass it to the fitCallbacks() as a parameter
* **Create a list containing text values with the names of the analytics you want to capture, i.e. [‘loss’, ‘val_loss’, ‘acc’, ‘val_acc’] and pass it to fitCallbacks() as a parameter**
> Correct

## Question 7
When using a dataset like MNIST or FashionMNIST, why is it advisable to use a sprite sheet containing all the images?
* It keeps the data in the native JS format
* It makes the data more secure
* It doesn’t require any additional pre-processing
* **It prevents excessive multiple HTTP calls to download the data**
> Correct

## Question 8
What is the role of tf.tidy() in TensorFlow.js?
* When it is executed, it removes everything tensorflow from the browser memory and cache
* It shuts down tensorflow when done, cleaning up all memory
* **When it is executed, it cleans up all intermediate tensors allocated by a function except those returned by the function**
* When it is executed it clears memory for new tensors
> Correct
