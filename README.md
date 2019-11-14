# Assignment for Programming for Data Analysis - November 2019
# Lecturer - Brian McGinley
# Submission Date - 11/11/19
# Objective - Create a jupyter notebook concerning the numpy.random package in Python and complete the tasks as outlined below.
# As per Assignment sheet;-
# There are four distinct tasks to be carried out in your Jupyter notebook. 
# 1. Explain the overall purpose of the package. 
# 2. Explain the use of the “Simple random data” and “Permutations” functions. 
# 3. Explain the use and purpose of at least ﬁve “Distributions” functions. 
# 4. Explain the use of seeds in generating pseudorandom numbers.
# To complete assignment the following base plan was created.
# a) Learn how to create a jupyter notebook and detail steps.
# b) Create the notebook and add to git repository.
# c) Expand on previous learnings of Python including the newer lecture content concerning NumPy and the numpy.random package.
# d) Use new learnings and the Jupyter notebook to complete the four tasks above.
# e) Complete Assignment to a suitable standard as per requirements outlined in the assignment sheet within the repository. 

# Step Description
# a)  Learn how to create a jupyter notebook and detail steps.
#  (i) Jupyter - "a loose acronym meaning Julia, Python, and R" (Datacamp, 2019) - The base languages jupyter was created to include but it now includes various other languages, including Python.
# (ii) Notebook - jupyter notebook versions allow the inclusion of code, graphs, figures, etc. in a single document repository and Datacamp (2019) state these document holdings "are the ideal place to bring together an analysis description, and its results, as well as, they can be executed perform the data analysis in real time".
# (iii) The Jupyter Notebook App - allows running the program on a web browser with the kernel and dashboard the primary components. The kernel deals with the code inputted by the user. The dashboard shows the high level of this access and allows creation or editing of notebooks and managing of kernels on the system you are using.
# How To Install Jupyter: - Using Anaconda to include the Python prerequisite requirement as highly recommended in class content and by Jupyter Documentation (2019). 
# Anaconda was previously installed but the following installation steps adapted by Jupyter Documentation (2019) should be followed.
# 1. Download Anaconda. It should include Anaconda’s latest Python 3 version (currently Python 3.7).
# 2. Follow the instructions on the download page. 
# 3. Complete the installation of Anaconda.
# 4. Open Command Line. (Cmder in this instance).
# 5. To run the notebook on the command prompt type: >>>> jupyter notebook

# (b) Create the notebook and add to git repository.

# GitHub account previously created on GitHub.com for creation of repositories of code, assignment and lecture content input. GitHub is the worlds leading software development and sharing platform which brings together the worlds greatest community of developers (GitHub.com, 2019).
# With the GitHub account created the following steps were followed to add a repository for assignment which included the Jupyter Notebook as outlined;
# a) New Repository Button on left hand side in profile view.
# b) Give Repository name, description, choose public/private, intialize the repository with a README file, choose .gitignore as Python and license as Apache License 2.0.
# c) The repository is created and now the Clone or Download link on right hand side was selected to copy the URL. 
# d) Pick destination folder on desktop and use command line to paste URL while syncing Git master - > origin folder.
# e) Once synced call >>> jupyter notebook. If it is previously installed as per steps the jupyter notebook will either open on the browser or you can copy and paste the URL which is contained within the command line.
# f) At the end of every edit or completion save the Jupyter checkpoint and close, press CTRL + C to close the kernel of the notebook on the commanad line and use git add ., git commit -m and git push to push changes from host to git repository.

# (c) Expand on previous learnings of Python including the newer lecture content concerning NumPy and the numpy.random package.

# NumPy is "the fundamental package supported for presenting and computing data with high performance in Python" Phuong and Czygan (2015, p. 11).
# Features, (list adapted from Phuong and Czygan, 2015);
# Built into Python.
# Multidimensional arrays (ndarrays).
# Other objects such as masked arrays, vectorization matrices, and broadcasting functions.
# Computational operations on arrays of data including mathematical manipulation, statistics, sorting, selecting, random number generation, Fourier transforms, etc.
# Integration with C/C++ and Fortran Code.

# Some key NumPy related terms which are discussed in the assignment are defined briefly here as adapted from Marsland (2015) and from class content;

# i) Arrays - basic data structure that is used and are called as functions with values passed in as a list or set of lists. >>> np.array().
# ii) Linear algebra - NumPy includes standard linear functions within its package, e.g. >>> np.linalg.inv(a) = getting the inverse of a.
# iii) Plotting - use of the Matplotlib library, imported as: >>> import matplotlib as pl. Most important are >>> pl.plot and >>> pl.hist which plot function as graphs or histograms respectively.
# iv) Pseudorandom Number Generator - abbreviated to PRNG - uses seed information to produce an algorithm which for generating a sequence of numbers which in turn approximates sequences of random numbers. 
# v) Pseudorandomness - process for producing predictable outcomes if given information or statistical randomness without.
# vi) Mersenne Twister - is a pseudorandom number generator (PRNG) and is widely used in software packages.
# vii) Gaussian distribution - also known as normal distribution is a common continuous probability distribution and is useful for determining random values as their distributions are unknown.

# The following shows the list of all subset functions of NumPy's numpy.random routine quoted from SciPy.Org's reference manual webpage titled: Random sampling (numpy.random). 
# [*each function called as x in numpy.random.()]

# Simple random data¶
# rand(d0, d1, ..., dn)	Random values in a given shape.
# randn(d0, d1, ..., dn) Return a sample (or samples) from the “standard normal” distribution.
# randint(low[, high, size, dtype]) Return random integers from low (inclusive) to high (exclusive).
# random_integers(low[, high, size]) Random integers of type np.int between low and high, inclusive.
# random_sample([size]) Return random floats in the half-open interval [0.0, 1.0).
# random([size]) Return random floats in the half-open interval [0.0, 1.0).
# ranf([size]) Return random floats in the half-open interval [0.0, 1.0).
# sample([size]) Return random floats in the half-open interval [0.0, 1.0).
# choice(a[, size, replace, p]) Generates a random sample from a given 1-D array
# bytes(length) Return random bytes.

# Permutations
# shuffle(x) Modify a sequence in-place by shuffling its contents.
# permutation(x) Randomly permute a sequence, or return a permuted range.

# Distributions
# beta(a, b[, size]) Draw samples from a Beta distribution.
# binomial(n, p[, size]) Draw samples from a binomial distribution.
# chisquare(df[, size]) Draw samples from a chi-square distribution.
# dirichlet(alpha[, size]) Draw samples from the Dirichlet distribution.
# exponential([scale, size]) Draw samples from an exponential distribution.
# f(dfnum, dfden[, size]) Draw samples from an F distribution.
# gamma(shape[, scale, size]) Draw samples from a Gamma distribution.
# geometric(p[, size]) Draw samples from the geometric distribution.
# gumbel([loc, scale, size]) Draw samples from a Gumbel distribution.
# hypergeometric(ngood, nbad, nsample[, size]) Draw samples from a Hypergeometric distribution.
# laplace([loc, scale, size]) Draw samples from the Laplace or double exponential distribution with specified location (or mean) and scale (decay).
# logistic([loc, scale, size]) Draw samples from a logistic distribution.
# lognormal([mean, sigma, size]) Draw samples from a log-normal distribution.
# logseries(p[, size]) Draw samples from a logarithmic series distribution.
# multinomial(n, pvals[, size])	Draw samples from a multinomial distribution.
# multivariate_normal(mean, cov[, size, ...) Draw random samples from a multivariate normal distribution.
# negative_binomial(n, p[, size]) Draw samples from a negative binomial distribution.
# noncentral_chisquare(df, nonc[, size]) Draw samples from a noncentral chi-square distribution.
# noncentral_f(dfnum, dfden, nonc[, size]) Draw samples from the noncentral F distribution.
# normal([loc, scale, size]) Draw random samples from a normal (Gaussian) distribution.
# pareto(a[, size]) Draw samples from a Pareto II or Lomax distribution with specified shape.
# poisson([lam, size]) Draw samples from a Poisson distribution.
# power(a[, size]) Draws samples in [0, 1] from a power distribution with positive exponent a - 1.
# rayleigh([scale, size]) Draw samples from a Rayleigh distribution.
# standard_cauchy([size]) Draw samples from a standard Cauchy distribution with mode = 0.
# standard_exponential([size]) Draw samples from the standard exponential distribution.
# standard_gamma(shape[, size]) Draw samples from a standard Gamma distribution.
# standard_normal([size]) Draw samples from a standard Normal distribution (mean=0, stdev=1).
# standard_t(df[, size]) Draw samples from a standard Student’s t distribution with df degrees of freedom.
# triangular(left, mode, right[, size]) Draw samples from the triangular distribution over the interval [left, right].
# uniform([low, high, size]) Draw samples from a uniform distribution.
# vonmises(mu, kappa[, size]) Draw samples from a von Mises distribution.
# wald(mean, scale[, size]) Draw samples from a Wald, or inverse Gaussian, distribution.
# weibull(a[, size]) Draw samples from a Weibull distribution.
# zipf(a[, size]) Draw samples from a Zipf distribution.

# Random generator
# RandomState Container for the Mersenne Twister pseudo-random number generator.
# seed([seed]) Seed the generator.
# get_state() Return a tuple representing the internal state of the generator.
# set_state(state) Set the internal state of the generator from a tuple.

# Reference List
# Class Content, Background Reading and Python Learning Tutorials were preliminary references supplemented by the following list of references;

# 1. Python Software Foundation. Accessed online at: https://www.python.org/
# 2. w3Schools.com Tutorials. Accessed online at: https://www.w3schools.com
# 3. Python by Programiz Tutorials. Accessed online at: https://www.programiz.com/
# 3. Pandas: Python Data Analysis Library. Accessed online at: https://pandas.pydata.org.
# 4. NumPy. Accessed online at: http://www.numpy.org
# 5. Stack Overflow - Various queries for comparison and improving code output. Accessed online at: https://stackoverflow.com
# 6. SciPy.org (2019) Random Sampling (numpy.random). Accessed online at: https://docs.scipy.org/doc/numpy-1.14.0/reference/routines.random.html
# 7. SciPy.org (2019) numpy.random.permutation. Accessed online at: https://docs.scipy.org/doc/numpy-1.14.0/reference/generated/numpy.random.permutation.html
# 8. SciPy.org (2019) Quickstart Tutorial. Accessed online at: https://docs.scipy.org/doc/numpy/user/quickstart.html
# 9. Numpy.org (2019) Random Sampling (numpy.random). Accessed online at: https://numpy.org/doc/1.17/reference/random/index.html
# 10. Jupyter Documentation (2019) Installing Jupyter Notebook. Accessed online at: https://jupyter.readthedocs.io/en/latest/install.html
# 11. DataCamp (2019) Tutorial on Jupyter Notebook Creation. Accessed online at: https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook?utm_source=adwords_ppc&utm_campaignid=898687156&utm_adgroupid=48947256715&utm_device=c&utm_keyword=&utm_matchtype=b&utm_network=g&utm_adpostion=1t1&utm_creative=332602034352&utm_targetid=dsa-473406581035&utm_loc_interest_ms=&utm_loc_physical_ms=20474&gclid=EAIaIQobChMIm_T_iu_S5QIVxLHtCh115QCvEAAYASAAEgKNHfD_BwE
# 12. Tutorialspoint (2019) NumPy Tutorial. Accessed online at: https://www.tutorialspoint.com/numpy/index.htm. 
# 13. NumPy Community (2017) NumPy User Guide. Accessed online at: https://numpy.org/doc/_downloads/numpy-user-1.13.0.pdf
# 14. Pynative (2019) Python Random Number Generation tutorial. Accessed online at: https://pynative.com/python-random-module/
# 15. Brownlee, J. (2018) How to Generate Random Numbers in Python. Machine Learning Mastery. Accessed online at: https://machinelearningmastery.com/how-to-generate-random-numbers-in-python/
# 16. Geeks for Geeks (2019) Random sampling in numpy | random_sample() function. Accessed online at: https://www.geeksforgeeks.org/random-sampling-in-numpy-random_sample-function/amp/
# 17. Phuong, V. T. H and Cyzgan, M. (2015) Getting Started with Python Data Analysis. Accessed online at: https://subscription.packtpub.com/book/big_data_and_business_intelligence/9781785285110/backindex
# Marsland, S. (2015) Machine Learning: An Algorithmic Perspective. Taylor and Francis Group.