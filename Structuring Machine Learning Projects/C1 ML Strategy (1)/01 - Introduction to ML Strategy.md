## Orthogonalization

To be able to easily achieve our goals, we need every control variables to be orthogonal to each other (not affecting each other)
for example: a car has 3 control variable which is steering, accelerating and breaking.

## Chain of Assumptions in ML
* Fit training set well on cost function
> first at least the training set is pass certain degree (i.e. a system that at least perform at human level performance) <br>
> If it's not doing well we can try bigger network or trying different optimization like adam

* Fit dev set well on cost function
> If it's not doing well we need a different control variables then the first step. we can try regularization or bigger training set

* Fit test well on cost function
> If it's not doing well in this step we need another control variables, we can try using a bigger dev set

* Performs well in real world
> Last if it's not doing well in this step we can try change either the dev set or the cost function
