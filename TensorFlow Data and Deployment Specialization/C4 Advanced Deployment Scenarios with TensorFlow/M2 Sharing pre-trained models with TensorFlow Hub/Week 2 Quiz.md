# Week 2 Quiz
## Latest Submission Grade: 100%

## Question 1
What’s the URL of the TensorFlow Hub site containing lots of models?
* Tensorflow.org/hub
* tensorflow.org/tfhub
* **Tfhub.dev**
* Tfdev.hub
> Correct

## Question 2
What are the primary problem domains for which you can find models on hub?
* Image and Computer Vision
* Text and NLP
* Video and Computer vision
* **All of the above**
> Correct

## Question 3
How do you install the Hub API in Python?
* Pip install tensorflow-hub
* Pip install tf-hub
* **Pip install tensorflow_hub**
* Pip install tf_hub
> Correct

## Question 4
When I have the URL of a model in MODULE_HANDLE, what’s the API to load it?
* model = open.hub(MODULE_HANDLE)
* **model = hub.load(MODULE_HANDLE)**
* model = hub.get(MODULE_HANDLE)
* model = hub.open(MODULE_HANDLE)
> Correct

## Question 5
In a transfer learning scenario, and a model was created using keras, how can you get the layer that you can freeze, and retrain everything beneath?
* hub.Freeze_Layer(...)
* hub.Get_Layer(...)
* hub.Keras(...)
* **hub.KerasLayer(...)**
> Correct

## Question 6
You’ve taken a keras layer from a hosted model in hub and called it ‘foo’. What’s the syntax to then build a DNN with foo as the top layer(s)?
* **model = tf.keras.Sequential([foo, Dense(2, activation='softmax')])**
* model = tf.keras.Sequential([foo)] + ([Dense(2, activation='softmax')])
* model = tf.keras.Sequential([Dense(2, activation='softmax'), foo])
* model = tf.keras.Sequential([foo], [Dense(2, activation='softmax')])
> Correct

## Question 7
If you want to use a model in TensorFlow Lite, how can you do it with Hub?
* Take a TFLite model from hub
* Take a general model from hub and convert to TF Lite
* Take layers from a hub model, retrain, and convert to TF Lite
* **All of the above**
> Correct

## Question 8
You download an embedding from tensorflow hub and want to retrain it, what do you do?
* Nothing -- it’s retrainable by default
* You can’t download an embedding
* **Use the trainable=true parameter in the KerasLayer call**
* Nothing -- you can’t retrain it
> Correct

## Question 9
If you want to get a JavaScript model from Hub, what’s the easiest way to do it?
* In TF.js use the KerasLayers method and pass it the model URL
* Download the savedmodel from hub and convert it using the TF Lite converter
* You can't do this
* **In TF.js use the loadGraphModel method and pass it the model url**
> Correct

## Question 10
You load a layer from hub using the KerasLayers method, and then add layers beneath it. When you do model.summary(), what will you see?
* All of the layers from the original model followed by your layers
* **A KerasLayer followed by your layers**
* You can’t do this for model privacy reasons
* A single layer from the original model followed by your layers
> Correct
