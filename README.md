# Maximum Likelihood Classification
  The main idea of Maximum Likelihood Classification is to predict the class label y that maximizes the likelihood of our observed data x. We will consider x as being a random vector and y as being a parameter (not random) on which the distribution of x depends. At first, we need to make an assumption about the distribution of x (usually a Gaussian distribution).

Then, the learning of our data consists of the following:
  - We split our dataset into subsets corresponding to each label y.
  - For each subset, we estimate the parameters of our assumed distribution for x using only the data inside that subset.

When making a prediction on a new data vector x:
  - We evaluate the PDF of our assumed distribution using our estimated parameters for each label y.
  - Return the label y for which the evaluated PDF had the maximum value.
    
    


