# Fundamentals of Data Analysis Tasks


This repository contains a jupyter notebook with four completed tasks for the Fundamentals of Data Analysis module. Each task has been given an individual section in the notebook, clearly marked with a heading, beginning with an explanation of the thought process behind methods of completing the task, followed by the code. The tasks got increasingly difficult, and required greater levels of complexity and detail in the code. 

Task 1 - Required a Python function called counts to be created, which takes a list as input and returns a dictionary of unique items in the list as keys and the number of times each item appears as values. The python dict() function was used for this task, a function which creates a dictionary, taking a list as input. The List.count() function is used to return a count of each key in the list. This task was relatively simple and required very minimal code.

Task 2 - Required a Python function called dicerolls to be created which simulates rolling dice. The function takes two parameters: the number of dice k, and the number of times to roll the dice n. The function simulates randomly rolling k dice n times, keeping track of each total face value, and returns a dictionary with the number of times each possible total face value occurred. Once the function and its parameters were defined, an empty dictionary was set up. This was followed by a for loop which used the random.choice function to select a side value of the rolled dice, and was carried out n times. The results of each roll in the loop were added to the empty dictionary. The function then returns a dictionary of results. This task required a defined function, the creation of a dictionary, and a standard for loop to return the desired output. 


Task 3 - Required us to write python code which simulates flipping a coin 100 times. The code will then be run 1,000 times, keeping track of the number of heads in each of the 1,000 simulations. An appropriate plot will be selected to depict the resulting list of 1,000 numbers, showing that it roughly follows a bell-shaped curve. The use of the numpy.binomial function was used for this task, which was relatively simple once the parameters were carefully selected. A binomial distribution describes the outcome of a binary scenario, a scenario with two possible outcomes. The numpy.random.binomial function has three parameters 1. n - number of trials 2. p - probability of occurence of each trial (e.g. for toss of a coin 0.5 each) 3. size - The shape of the returned array (w3schools, 2020). We set the probability (p) to 0.5, the number of trials (n) to 100, and size to 1000 to get the desired output as specified. In order to plot the output and show that it roughly follows a bell-shaped curve, we used the seaborn.distplot function. Setting hist = true, sets the plot as a histogram, and kde = true, plots a gaussian kernel density estimate. Once the output of the coin flip is run through this function, the bell-shaped curve is clearly observed.


Task 4 - Deals with Simpson’s paradox, a well-known statistical paradox which occurs when a trend or result that is present when data is put into groups, reverses or disappears when the data is combined (Grigg, 2018). This task requires us to use numpy to create four data sets, each with an x array and a corresponding y array, to demonstrate Simpson’s paradox. To clearly understand Simpson's paradox we create the four data sets, plot them on one graph to show the positive x, y correlation and slope, and then add a combined best fit line to show the presence of Simpson's paradox. Four x arrays are created using the numpy.linspace function to return evenly spaced numbers over a specified interval. To create a y array to correspond with the x array, we use the equation y = a * x + b. This equation is a linear equation in slope-intercept form. We then add some random numbers from the normal distribution, to add noise to the array. When the four x and y arrays are created, we use the numpy.polyfit function to get the coefficients of each set of axis, which will be used to plot the best fit line of each set. Then we simply plot each of the 4 sets of arrays, along with their best fit lines, to compare their slopes. Finally, we concatenate each x array and y array using the numpy.concatenate function, and use the polyfit function to get the coefficient so that we can plot the combined best fit line of the data set. The combined best fit line is added to the plot of the 4 seperate arrays, providing a visual representation of Simpson's paradox.


The four tasks provided a good challenge, and were beneficial in my development as a data analyst. The first two tasks required careful thought and the creation of functions, while tasks three and four required me to learn new code, functions and expand my knowledge of data analytics. To ensure that I succesfully completed the assignment before the deadline, I consistently carried out research and started each task as soon as i had developed the required skills to do so. All the research which have helped shape my code and development are linked below. 






# Bibliography 

Arditi, A. (2020) 'Understanding Simpson’s Paradox to Avoid Faulty Conclusions' Sisense. Available at: https://www.sisense.com/blog/understanding-simpsons-paradox-to-avoid-faulty-conclusions/ Accessed on: 01/12/2020.

Dargan, J. (2020) 'Create a Dictionary From a List' Medium. Available at: https://medium.com/swlh/create-a-dictionary-from-a-list-65742246ab4b Accessed on: 03/11/2020.

Fuentes, A. (2018) 'Using NumPy for Simulations' Vitosh Academy. Available at: https://www.vitoshacademy.com/using-numpy-for-simulations/ Accessed on: 10/11/2020.

Grigg, T. (2018) 'Simpson’s Paradox and Interpreting Data' Towards Data Science. Available at: https://towardsdatascience.com/simpsons-paradox-and-interpreting-data-6a0443516765 Accessed on: 02/12/2020.

Haddad, A. (2020) 'Python Return Multiple Values – How to Return a Tuple, List, or Dictionary' Free Code Camp. Available at: https://www.freecodecamp.org/news/python-returns-multiple-values-how-to-return-a-tuple-list-dictionary/ Accessed on: 29/10/2020.

Kievit, R., Frankenhuis, W.E., Waldorp, L. and Borsboom, D. (2013) 'Simpson's paradox in psychological science: a practical guide' Frontiers in psychology. Available at: https://www.frontiersin.org/articles/10.3389/fpsyg.2013.00513/full Accessed on: 12/12/2020.

Koehrsen, W. (2018) 'Simpson’s Paradox: How to Prove Opposite Arguments with the Same Data' Towards Data Science. Available at: https://towardsdatascience.com/simpsons-paradox-how-to-prove-two-opposite-arguments-using-one-dataset-1c9c917f5ff9 Accessed on: 2/12/2020.

Kumar, V. (2020) 'Making Dice Rolling Game Via Python Code' Medium. Available at: https://medium.com/@vishalkumar240107/making-diec-rolling-game-via-python-code-409efa1f9b9c Accessed on: 04/11/2020.

Kundycki, J. (2020) 'Use Python to build a Dice Roller App' Towards Data Science. Available at: https://towardsdatascience.com/use-python-to-build-a-dice-roller-app-2408e66bf009 Accessed on: 25/11/2020.

Salmon, M. (2017) 'Probability in a Weighted Coin-flip Game using Python and Numpy' Towards Data Science. Available at: https://towardsdatascience.com/probability-in-a-weighted-coin-flip-game-using-python-and-numpy-bc1686c49a35 Accessed on: 28/11/2020.

Seaborn. (2020) 'seaborn.kdeplot' Seaborn. Available at: https://seaborn.pydata.org/generated/seaborn.kdeplot.html#:~:text=A%20kernel%20density%20estimate%20 Accessed on: 02/12/2020.

Sturtz, J. (2020) 'Dictionaries in Python' Real Python. Available at: https://realpython.com/python-dicts/ Accessed on: 01/11/2020.

Umayanga, T. (2020) 'What is Binomial Distribution and how to Plot it using Python' Medium. Available at: https://medium.com/@tharakau/what-is-binomial-distribution-and-how-to-plot-it-using-python-e9d95bd341ee Accessed on: 2/12/2020.

W3Schools. (2020) 'Python Random choices() Method' W3Schools. Available at: https://www.w3schools.com/python/ref_random_choices.asp Accessed on: 01/12/2020.

W3Schools. (2020) 'Binomial Distribution' W3Schools. Available at: https://www.w3schools.com/python/numpy_random_binomial.asp Accessed on: 25/11/2020.

Wang, B., Wu, P., Kwan, B., Tu, X. M., & Feng, C. (2018). Simpson's Paradox: Examples. Shanghai archives of psychiatry. Available at: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5936043/ Accessed on: 01/12/2020.
