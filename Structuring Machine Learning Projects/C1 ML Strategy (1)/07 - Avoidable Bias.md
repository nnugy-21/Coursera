## Avoidable Bias

In the example below we have training and dev accuracy compared to human level accuracy. <br>
What we are trying to achieve here is to choose which function should we improve.

In the example below we can see that, on the left side the difference in accuracy between our model and human level is 7% **This is called Avoidable Bias**, and the difference between training set and dev set only 2%. <br>
With that we can decide to reduce the difference between training set and human level rather than training set and dev set. <br>
We can do it by focusing on the bias.

On the other example, the difference between training and dev set is higher than the **Avoidable Bias**. <br>
That way we can focus more on modifying the variance between training set and dev set, or we can try to input more data in training set.

![image](https://user-images.githubusercontent.com/79896959/114706959-db2df280-9d53-11eb-8faa-6d6c89f8109a.png)
