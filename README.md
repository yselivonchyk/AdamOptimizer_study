# AdamOptimizer_study

The purpose of this study is to visualize behavior of AdamOptimizer algorithm on trivial functions and argue about direct effects of the parameter choice.

[Original paper](https://arxiv.org/abs/1412.6980)

## Dependencies
* Python 3
* Numpy
* Matplotlib

## Results
In the course of the experiments next tendencies were observed:
* Normalization of zero-bias leads to more "stable" updates earlier in the learning. i.e. while few update values were observed
* Algorithm smooths the function of update values over time
* Algorithm normalizes updates to closer match the learning rate
* Algorithm does not cause decrease in update values over time
* Value of epsilon is of little importance. The only significant observed for large values of epsilon and can be achieved by changing the learning rate proportionally

Shortcomings of the study:
* Effects (and, therefore, rules) of second order moment (v) are not clear. The only special case observed in the studies is B1=B2.