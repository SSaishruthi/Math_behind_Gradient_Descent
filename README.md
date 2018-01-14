# Gradient_Descent

There are many ways to frame the learning process. Easiest way is to use labelled data. For a given input, it is necessary to learn how these are mapped to the output. To measure the performance, an error function is defined. 

Given an input, prediction is made. This prediction is then compared with the actual output and their difference will give the accuracy of the model. Parameters used for the predictions must be updated during every iteration. Parameters are changed until the system learns mapping and gives significant decrease in the error value.

Updating parameter is called optimization. Here is an example which has x-y pairs, where ‘x’ represents the distance a person travels in bike and ‘y’ represents the number of calories that they have lost. 


Task is to find a function that can effectively map the input to output. Since, the data points are scattered it is not possible to represent it using a straight-line equation. Best solution is to draw a line that will best fit and pass through as many as data points as possible. 
Equation of straight line,
              Y = mx + b
Here,
‘m’ is the slope
‘b’ is the intercept

Optimum value for ‘b’ and ‘m’ must be found so that the obtained line can best fit as many as data points possible and also output obtained from these values will be nearly equal to the actual value.

Error Function
SSE (Sum of Squared Error) = ∑(Actual value-Predicted Value)^2
SSE (Sum of Squared Error) = 1/N ∑_(i=1)^n▒〖(Actual Output-((Slope*x)+intercept))^2  〗
                             1/N ∑_(i=1)^n▒〖(y-((m*x)+b))^2  〗

Summing up all the errors can give final error value for the function. Initially ‘b’ and ‘m’ are assigned 0.

Iterating through different values of slope and intercept can yield different error values. Out of all values, there will be one point where error value will be minimum and parameters corresponding to this value will yield the optimal solution.

Now, how to descend in this graph to reach the minimum point. Finding the slope at a given point can do this. This slope will point in a direction that can lead to the minimum of the graph. 

In calculus, this is called derivative of a function. Partial derivative with respect to both ‘b’ and ‘m’ are calculated.

Partial derivate with respect to ‘b’ 
2/N ∑_(i=1)^n▒〖-(y-(mx+b)) 〗

Partial derivative with respect to ‘m’
2/N ∑_(i=1)^n▒〖-x(y-(mx+b))  〗

When,
‘b’ and ‘m’ are 0, error value is 5565.11
After 950 iterations, 
‘b’ value is 1.52484 
‘m’ value is 0.0606 
Error value is 112.76
