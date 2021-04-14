## Single Number Evaluation Metric

* Precision = The times that our classifier recognize a cats, what percentage actually are cats?
> So, if classifier A recognize a cat, it has 95% chance it actually a cat

* Recall = Of all the images of really are cats, what percentages are actually recognize by the classifier?
> So, if classifier A has 90% Recall, it means it recognize 90% of the actual cats images.

![image](https://user-images.githubusercontent.com/79896959/114687373-e413c980-9d3d-11eb-8efd-3f6be6afaa4e.png)

But in the example above, classifier A has a better Recall and classifier B has a better Precision, so which one should we choose? <br>
Because of that, we need another metric which is F1. <br>
F1 = the harmonic mean of Precission and Recall <br>
**So, what we are trying to say here, if u want to evaluate ur system, it's better if u have 1 single number evaluation metric to measure it easily**
![image](https://user-images.githubusercontent.com/79896959/114688681-21c52200-9d3f-11eb-8334-d4edbe106d59.png)
