# Week 1 Quiz
## Latest Submission Grade: 100%

## Question 1
What platforms are supported by TensorFlow Lite (Check all that apply)
* **Android**
> Correct
* Windows Phone
* **Some Microcontrollers**
> Correct
* **iOS**
> Correct
* **Raspberry Pi**
> Correct

## Question 2
What is Quantization?
* A technique that increases precision to ensure your model works better on mobile
* A technique to ensure compatibility across all supported platforms
* **A technique that reduces precision and model size to work better on mobile**
* A technique to optimize the size of a model for the memory map of a mobile device
> Correct

## Question 3
The TFLite file format is an example of what?
* A savedmodel
* A checkpoint
* A concrete function
* **A flatbuffer**
> Correct

## Question 4
Which types of input does the TF Lite Convertor API Accept (Check all that apply)
* **A SavedModel**
> Correct
* **A Keras HDF5 file**
> Correct
* **A set of concrete functions**
> Correct
* A model object
* A list of checkpoints

## Question 5
True or False: The SavedModel format supports model Versioning
* **True**
* False
> Correct

## Question 6
If I want to save an existing Keras model, what’s the API signature:
* **tf.saved_model.save(model, path)**
* tf.save(model, path)
* tf.saved_model.path=path
* Tf.model.save(path)
> Correct

## Question 7
If I want to use the TensorFlow Lite Convertor to convert a saved model to TF Lite, what’s the API signature?
* newModel = tf.lite.TFLiteConverter.convert(model_path)
* newModel = tf.lite.TFLiteConverter.fromModel(myModel).convert()
* **converter = tf.lite.TFLiteConverter.from_saved_model(path)<br>
newModel = converter.convert()**
* converter = tf.lite.TFLiteConverter.convert()<br>
newModel = converter.Convert(model_path)
> Correct

## Question 8
If I have a keras model and want to convert it, what’s the method signature on TFLiteConverter
* from_keras(model)
* convert(model)
* **from_keras_model(model)**
* convert_keras_model(model)
> Correct

## Question 9
If I want to convert using a command line tool, what’s the name of the tool?
* tfliteconvert
* **tflite_convert**
* Tflite_to_model
* tf_convert_lite
> Correct

## Question 10
If I want to do post training quantization, what are the optimization options available (check all that apply)
* OPTIMIZE_FOR_ANDROID
* OPTIMIZE_FOR_IOS
* OPTIMIZE_FOR_PERFORMANCE
* **OPTIMIZE_FOR_SIZE**
> Correct
* **OPTIMIZE_FOR_LATENCY**
> Correct
