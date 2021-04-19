# Quiz 1
## Latest Submission Grade: 100%

## Question 1
What is the name of the API at the heart of TensorFlow.js which allows things like layers to be used?
* TFJS API
* JS API
* Core TF API
* **Core API**
> Correct

## Question 2
How does TensorFlow.js use GPU acceleration in the browser?
* **You access GPU through WebGL in the browser**
* It works natively through GPU libraries in TensorFlow
* It doesn’t
* You have to install GPU runtimes for each browser, and explicitly use them
> Correct

## Question 3
How can you use a TPU with TensorFlow.js?
* You can't
* You have to serve your JS from a GCP instance
* **You can use Node.js on GCP and access TPU instances**
* Only using Colab
> Correct

## Question 4
Which of the following lines of code will correctly add a single dense layer containing a single neuron that takes a numeric input to a model using JavaScript?
* **model.add(tf.layers.dense({units: 1, inputShape: [1]}));**
* model.add(tf.layers({units: 1, inputShape: [1,1]}))
* model.add(tf.layers.dense({units: 1, inputShape:= [1]}));
* model.add(tf.layers.dense({units= 1, inputShape: [1]}));
> Correct

## Question 5
When creating data to input to a model using Python you could use a numpy array. How would you do it in JavaScript?
* **Use a tensor2d containing the data and the shape of the data**
* Use a tensor2d containing the data
* Use a numpyjs array
* Use a tensor2d contining a numpyjs array
> Correct

## Question 6
If I train a model to detect a linear relationship (i.e. Y=2X-1), what line of code would output a prediction from that model for Y where X=10?
* **alert(model.predict(tf.tensor2d([10], [1,1])));**
* alert(model.predict([10], [1,1]));
* alert(model.predict(10));
* alert(model.predict(tf.tensor2d([10])));
> Correct

## Question 7
When training a model, if I want to log training status at the end of an epoch, what is the name of the callback event you want to capture?
* OnEpochEnded
* EpochEnd
* EpochEnded
* **OnEpochEnd**
> Correct
