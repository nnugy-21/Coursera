## Satisficing and Optimizing Metric

Sometimes, it really hard to combine 2 metric into Single Number Evaluation Metric like the example below. <br>
In that case, we can separate those two metric into two group:
* Optimizing Metric = The metric u really care about
> In the example below, the optimizing metric are **Accuracy** for cat classifier and **Accuracy** for Trigger Words
* Satisficing Metric = The metric that only need to be at least pass certain condition
> In the example below, the satisficing metric are **Run time** for cat classifier and **False Positive** for Trigger Words

So, in the cat example we can set the optimizing metric as **the one that has the highest accuracy** and satisficing metric as **at least the run time is below 100ms**. Because of that **we can pick Classifier B as the best Classifier** for Cat Classifier

![image](https://user-images.githubusercontent.com/79896959/114691679-217a5600-9d42-11eb-9326-d16c5cc6139f.png)
