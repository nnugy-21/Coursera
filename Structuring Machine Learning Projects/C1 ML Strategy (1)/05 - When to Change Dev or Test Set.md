## When to Change the Dev or Test Set

In the example below we have Classifier A that performs better than Classifier B, but Classifier A although only has 3% error it let through some pornographic images, which is unacceptable. <br>
So, our company and users prefer the Classifier B. So, what should we do?
<br>
What we can do is to change our metric formula, in the example below, we can see our original error function written in blue color. So, we can add some weight which was written in red color. If the images is pornographic it will be 10 weights and if its not it will only has 1 weight. So, when they training or detecting the pornographic images, they will return a high error value.
![image](https://user-images.githubusercontent.com/79896959/114696950-78365e80-9d47-11eb-831a-aa086f7448f0.png)
