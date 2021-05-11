# Week 4 Quiz
## Latest Submission Grade: 100%

## Question 1
What advantage does Federated Learning give you?
* User data can remain private on their device but still be used to train models
* Users can have models trained on everybody’s data
* Models can be frequently updated
* **All of the above**
> Correct

## Question 2
What is the privacy principle of focused collection?
* Engineer filters all the data to get only what she needs for a calculation
* Data is filtered by the network to remove all irrelevant data
* Devices filter all the data from the server to only use updates
* **Devices report only the data needed for a specific computation**
> Correct

## Question 3
What is secure aggregation?
* Devices in a network pair up, and aggregate mutual data before sending to the server
* Data is aggregated before being sent to the server, and only sent on encrypted channels
* **Devices in a network pair up, and create obfuscation keys that get cancelled out when aggregated on the server**
* Data is aggregated on the device before sending to the server, and sent on an encrypted channel
> Correct

## Question 4
TensorFlow Federated includes a Federated Learning API, a Federated Core API and a runtime for simulations. What’s the role of the Federated Learning API?
* It is a mobile runtime for Federated Learning
* It’s designed to allow the expression of new Federated algorithms
* **It contains implementations of federated training that can be applied to existing tensorflow models and data**
* It is the API for everything Federated Learning
> Correct

## Question 5
If you want to declare a federated type, where a numeric item of data is available across all your devices, how do you do it?
* Each device needs the same variable name and type
* You declare the type as {float32}@server
* **You declare the type as {float32}@clients**
* You can’t do this for privacy reasons, you have to declare it when submitting to the server
> Correct

## Question 6
If you want to do a federated computation on the server, what do you need to do to your computation function?
* Make sure it returns its value to @Clients
* **Attribute the function with @tff.federated_computation**
* Attribute the function with @federated
* Nothing, it will just work automatically
> Correct

## Question 7
You want to return a mean value of client values, calculated on the server, back to the clients. How do you do this?
* You have to explicitly open a network pipe and send the value to all of the clients using it
* The return value from your function is automatically mapped to the clients
* You can’t do this for privacy reasons
* **You have to use a tff.federated_mean to calculate the value and return its results**
> Correct

## Question 8
If you want to try the tensorflow federated APIs, how do you install them for Python?
* **Pip install tensorflow_federated**
* Do nothing, they’re included in TensorFlow
* Pip install tensorflow-federated
* Pip install tf-federated
> Correct
