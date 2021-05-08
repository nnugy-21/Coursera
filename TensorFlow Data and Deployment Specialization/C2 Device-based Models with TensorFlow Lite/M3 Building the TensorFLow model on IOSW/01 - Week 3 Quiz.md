# Week 3 Quiz
## Latest Submission Grade: 100%

## Question 1
What technology is used to deploy addons like TensorFlow Lite to iOS applications?
* Gradle
* **Cocoapods**
* Applepods
* VSNs
> Correct

## Question 2
What is the name of the pod that you use to add TF Lite to an iOS app with the Swift language?
* **TensorFlowLiteSwift**
* TensorFlowSwift
* TensorFlowLite
* LiteSwift
> Correct

## Question 3
How do you deploy a model to iOS for offline use?
* You bundle model and interpreter as a resource file
* You download it at runtime
* **You add is as part of the app bundle**
* You convert it to swift code and use it as an activity
> Correct

## Question 4
How does iOS represent images in memory?
* An array of bytes
* Image class
* **A CVPixelBuffer**
* An NSPixelArray
> Correct

## Question 5
How do you do inference with a TF Lite interpreter in Swift?
* interpreter.run(input, output)
* **Copy values to input tensor, call interpreter.invoke(), copy outputs to output Tensor**
* interpreter.invoke(input, output)
* Copy values to input tensor, call interpreter.run(), copy outputs to output Tensor
> Correct

## Question 6
How do you specify the number of threads that the interpreter should use?
* Use an InterpreterOptions object and set its threads property to the desired amount
* Call the setThreads() method on an InterpreterOptions object and specify the desired amount
* **Use an InterpreterOptions object and set its threadCount property to the desired amount**
* Use an InterpreterOptions object and set it’s useThreads property to true
> Correct

## Question 7
What format is an image in a CVPixelBuffer?
* **BGRA_32**
* RGBA_32
* BGR_32
* RGB_32
> Correct

## Question 8
How can you tell if a model is quantized at runtime?
* Check the isQuantized property on the interpreter. If it is true, the model is quantized
* **Check the inputTensor Data type. If it’s uInt8, the model is quantized**
* Check the isQuantized property on the input tensor. If it is true, the model is quantized
* Check the modelFormat data type. If it’s uInt8, the model is quantized
> Correct

## Question 9
In what order does the object detection model report the bounding box parameters?
* x, y, width, height
* **y, x, height, width**
* y, x, width, height
* x, y, height, width
> Correct
