Program  2

The first step is to  import libraires which will be used to calculate mean, variance and other statistical measures easier. \
The imported modules include:\
1.Numpy - It is used for numerical operations and random data generation.\
2.Matplotlib.pyplot - It used to visualize the probability distributions.\
3.Scipy - It provides functions for distributions such as: stats.binom ; stats.poisson ; stats.geom.

<img width="431" height="175" alt="image" src="https://github.com/user-attachments/assets/b517499a-5473-4a53-983f-673d86061ba0" />

Then the second step is to use the command “np.random.seed(42)” makes all subsequent "random" outputs completely reproducible.\
NOTE:The number inside can be changed its up to the person programming but 42 is used among most programmers.

PART 1: BINOMIAL DISTRIBUTION
Binomial Distribution is counting the number of successes in a fixed number of independent trials.\
Its denoted  by:   X ~ Binomial(n, p)		where, n = no. of trials\
							                                 p = probability of success

<img width="682" height="418" alt="image" src="https://github.com/user-attachments/assets/8d813eab-f34a-4519-96a8-cb1fbbf75466" />

Explanation of code\
Line 3: We are defining the parameters by setting n = 20 and p = 0.35.\
Line 4: We are defining a binomial distribution with parameters n and p.\
Line 5: We are creating a array with all possible outcome from 0 to 20.\
Line 6: We are calculating the mean using the predefined function in Scipy and theoretically calculating using formula.\
Line 7: We are calculating the variance using the predefined function in Scipy.\
Line 8: We are calculating the second moment and due to that inside the parentheses we are specifying 2.\
Line 9: We are calculating the skewness using binom.stats(“s”), s is used since we are trying to find the skewness if we change the value then another measure will be calculated instead.\
Line 10: We can directly find the cdf using .cdf function.\
Line 11: We can directly find the pmf using .pmf function.\
Line 13: From this line onwards we are visualizing the binomial distribution.\
Line 14: This line initializes a new plot figure with a width of 7 in. and height of 5 in.
Line 15: This plots a bar graph of the pmf distribution and the line,	“color='steelblue',edgecolor='black', alpha=0.8” tells the graph style.\
Line 16: This line marks the mean value(7) on the chart with a dashed red line.\
Line 17,18,19: These lines set the title and label the x and y axis.\
Line 20: This line displays the legend box.\
Line 21: This line helps add see-through horizontal lines across the chart to ease tracing and read the heights or values.\
Line 22,23: It adds spacing so no labels or titles get cut off, then opens the window to display the finished chart.

PART 2: POISSON DISTRIBUTION

Poisson Distribution is counting the number of events occurring within a fixed interval of time or space.\
Its denoted  by:   X ~ Poisson(λ)		where, λ = average rate of occurrence

<img width="692" height="381" alt="image" src="https://github.com/user-attachments/assets/7b41bb2a-7af7-4ddf-b2d4-9f6d9a1492e6" />

Explanation of code\
Line 2: We iterate through a list of different lambda values ( λ= 1, 3, 5, 10) using a for loop. \
Line 3: We are defining a Poisson distribution object with the parameter lam using the Scipy stats module. \
Line 4: We generate 5,000 random samples from the Poisson distribution to simulate the process. \
Line 5: Prints the current value of λ being analyzed. \
Line 6: We are calculating the theoretical mean using the predefined .mean() method from Scipy. \
Line 7: We calculate the empirical mean from the 5,000 generated simulation values using .mean() from NumPy. \
Line 8: Prints an empty line for clean spacing between iterations. \
Line 10: From this line onwards we are visualizing the Poisson distribution. \
Line 11: This line initializes a new plot figure with a width of 7 in. and height of 5 in. \
Line 12: We create an array x_p containing integer values from 0 to 19 to represent the possible count of events. \
Line 13: A for loop runs through the same list of λ values to plot a curve for each one. \
Line 14: This line calculates and plots the PMF for each outcome in x_p, with circular markers of size 4 and a distinct label for the legend. \
Line 15,16, 17: These lines set the title and label the x and y axis.\
Line 18: This line displays the legend box to differentiate the lines for each λ value. \
Line 19:  This line helps add see-through horizontal lines across the chart to ease tracing and read the heights or values.\
Line 20, 21: It adds spacing so no labels or titles get cut off, then opens the window to display the finished chart.\


PART 3: GEOMETRIC DISTRIBUTION

Geometric Distribution is modeling the number of trials needed to get the first success in repeated independent Bernoulli trials.\
Its denoted by:X ~ Geometric(p)	     where, p = probability of success in each trial

<img width="802" height="456" alt="image" src="https://github.com/user-attachments/assets/386d3b4a-edb5-4b74-b61c-9999f4436c58" />

Explanation of code\
Line 3: We are defining the parameter by setting the probability of success as 0.3. \
Line 4: We are defining a geometric distribution object with parameter p_geo using the Scipy stats module. \
Line 5: Prints a header indicating the distribution type and the assigned value of p. \
Line 6: We are calculating the mean using the predefined .mean() function in Scipy. \
Line 7: We can directly find the probability that the first success occurs on the 1st trial, P(X=1), using the .pmf() function. \
Line 8: We calculate the probability of the first success taking strictly more than 5 trials, P(X > 5), by taking “1 - geo.cdf(5)”. \
Line 10: From this line onwards we are visualizing the geometric distribution. \
Line 11: This line initializes a new plot figure with a width of 7 in. and height of 5 in. \
Line 12: We are creating an array with trial numbers ranging from 1 up to 19. \
Line 13: This plots a bar graph of the pmf distribution where color='green', edgecolor='black', and alpha=0.8 define the graph style. \
Line 14,15, 16: These lines set the title and label the x and y axis.\
Line 17: This line helps add see-through horizontal lines across the chart to ease tracing and read the heights or values.\
Line 18, 19: It adds spacing so no labels or titles get cut off, then opens the window to display the finished chart.
