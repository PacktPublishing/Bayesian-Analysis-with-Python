# Bayesian Analysis with Python

This is the code repository for [Bayesian Analysis with Python](https://www.packtpub.com/big-data-and-business-intelligence/bayesian-analysis-python?utm_source=github&utm_medium=repository&utm_campaign=9781785883804), published by Packt. It contains all the supporting project files necessary to work through the book from start to finish.


## Instructions and Navigations

All of the code is organized into folders. Each folder starts with a number followed by the application name. For example, Chapter02.


The code will look like the following:
```
n_params = [1, 2, 4]
p_params = [0.25, 0.5, 0.75]
x = np.arange(0, max(n_params)+1)
f, ax = plt.subplots(len(n_params), len(p_params), sharex=True, 
  sharey=True)
for i in range(3):
    for j in range(3):
        n = n_params[i]
        p = p_params[j]
        y = stats.binom(n=n, p=p).pmf(x)
        ax[i,j].vlines(x, 0, y, colors='b', lw=5)
        ax[i,j].set_ylim(0, 1)
        ax[i,j].plot(0, 0, label="n = {:3.2f}\np = 
         {:3.2f}".format(n, p), alpha=0)
        ax[i,j].legend(fontsize=12)
ax[2,1].set_xlabel('$\\theta$', fontsize=14)
ax[1,0].set_ylabel('$p(y|\\theta)$', fontsize=14)
ax[0,0].set_xticks(x)
```

This book is written for Python version >= 3.5, and it is recommended that you use 
the most recent version of Python 3 that is currently available, although most of the 
code examples may also run for older versions of Python, including Python 2.7 with 
minor adjustments.

Maybe the easiest way to install Python and Python libraries is using Anaconda, 
a scienti fi c computing distribution. You can read more about Anaconda and 
download it [here](https://www.continuum.io/downloads). Once Anaconda is in 
our system, we can install new Python packages with this command: 

```conda install NamePackage```

We will use the following python packages:


* Ipython 5.0
* NumPy 1.11.1
* SciPy 0.18.1
* Pandas  0.18.1
* Matplotlib 1.5.3
* Seaborn 0.7.1
* PyMC3 3.0

## Errata

If you find an error in the book please fill an issue or send a PR [here](https://github.com/aloctavodia/BAP)
=======
•  Ipython 5.0
•  NumPy 1.11.1
•  SciPy 0.18.1
•  Pandas  0.18.1
•  Matplotlib 1.5.3
•  Seaborn 0.7.1
•  PyMC3 3.0


## Related Products
* [Expert Python Programming](https://www.packtpub.com/application-development/expert-python-programming?utm_source=github&utm_medium=repository&utm_campaign=9781847194947)

* [Learning Bayesian Models with R](https://www.packtpub.com/big-data-and-business-intelligence/learning-bayesian-models-r?utm_source=github&utm_medium=repository&utm_campaign=9781783987603)

* [Mastering Probabilistic Graphical Models Using Python](https://www.packtpub.com/big-data-and-business-intelligence/mastering-probabilistic-graphical-models-using-python?utm_source=github&utm_medium=repository&utm_campaign=9781784394684)
### Suggestions and Feedback
[Click here](https://docs.google.com/forms/d/e/1FAIpQLSe5qwunkGf6PUvzPirPDtuy1Du5Rlzew23UBp2S-P3wB-GcwQ/viewform) if you have any feedback or suggestions.
