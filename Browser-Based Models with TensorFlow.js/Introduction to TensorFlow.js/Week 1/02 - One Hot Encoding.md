# One-Hot Encoding
## Latest Submission Grade: 100%

## Question 1
Given a set of Xs and Ys, how would you one-hot encode a label based on the text or ‘rock’, ‘paper’, ‘scissors’ ?
* trainingData.map(({xs, ys}) => {
    const labels = [ ys.label == ? 1 : 0, "rock", ys.label == ? 1 : 0, "paper",  ys.label == ? 1 : 0, "scissors"]
}

* **trainingData.map(({xs, ys}) => {
    const labels = [ ys.label == "rock" ? 1 : 0, ys.label == "paper" ? 1 : 0,  ys.label == "scissors" ? 1 : 0 ]
}** 

* trainingData.map(({xs, ys}) => {
    const labels = [ ys.label == "rock",  "paper", "scissors" ]
}

* trainingData.map(({xs, ys}) => {
    const labels = [ ys.label == "rock" == 1, ys.label == "paper" == 1,  ys.label == "scissors" == 1 ]
} 

> Correct
