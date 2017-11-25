## Welcome to CISC 5420 - Applied Statistics & Probability!

### Interesting Dataset
---
I came across an interesting dataset on home prices while reading this interesting New York Times article, [How much income do you need to buy a home?](https://www.nytimes.com/2017/11/23/realestate/how-much-income-do-you-need-to-buy-a-home.html?action=click&pgtype=Homepage&clickSource=story-heading&module=real-estate-left-region&region=real-estate-left-region&WT.nav=real-estate-left-region). The dataset from hsh.com shows the annual income one needs to be able to afford a home in one of America's 50 most populous cities. Check out the article and dataset [here](https://www.hsh.com/finance/mortgage/salary-home-buying-25-cities.html#_).

Let's talk about this information in class on Tuesday!

### Lecture 11
---
This week we spoke about statistical hypothesis testing - the methodology by which we determine whether the effects we see in a sample of data are likely to appear in a larger population. In hypothesis testing, the main question we seek to answer is "Given a sample and an apparent effect, what is the probability of seeing such an effect by chance?" (quote from Downey, ThinkStats2). This question captures the essence of hypothesis testing very nicely. Our "apparent effect" is quantified via a **test statistic**, the "by chance" part is modeled by the **null hypothesis**, and the "probability of such an effect by chance" is our **p-value**. The higher that probability (ie a high p-value) the higher the probability that the effect is due to random chance and hence not true of the larger population. 

Your homework assignment for next class is to read chapter 11 of ThinkStats2. Note, we will be covering chapter 10 on Linear Regression next week in class. We will cover chapter 11 next Saturday during our Skype class.

Happy Thanksgiving!

### Lecture 10
---
This week we discussed estimation - the process of estimating a population paramater such as the mean from a finite sample of data. In particular, we noted that how you estimate a parameter depends on the particular circumstance. For example, if your data comes from a normal distribution, than the sample mean is the best unbiased estimator, that is, it minimizes the [Mean Squared Error](https://en.wikipedia.org/wiki/Mean_squared_error). We also discussed [Maximum Likelihood Estimation](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation)(MLE) in depth. If we have a fixed dataset and statistical model, MLE selects the parameters that maximizes the likelihood function, i.e. maximizes the chance of observing the given data. We showed that 1/mean(x), (where mean(x) is the sample mean) is the MLE of the parameter lambda for the exponential distribution.

[Bias](https://en.wikipedia.org/wiki/Bias_of_an_estimator) is the difference between an estimator's *expected value* (i.e. average) and the true value of a parameter. An estimator with zero bias is *unbiased*. We showed computationally that the sample mean is an unbiased estimator of a Gaussian distribution.

Your homework assignment for next class is as follows:

  1. Read Ch. 9 and 10 of ThinkStats2 and run through the code in the chapter. These chapters discuss hypothesis testing and single linear regression - both very important topics. In particular, hypothesis testing is used to determine whether observed statistical differences, such as the observed mean difference in birth lengths between first babies and others, can be attributed to random chance. You will be asked to perform at least 2 hypothesis tests in your final projects so please read this chapter carefully.
  
  2. Check out [gmaps](https://github.com/pbugnion/gmaps), a Python package for plotting geographical data on Google Maps in the Jupyter notebook.
  
  3. We will not have class next week. Instead, we will make up lecture over a Skype lecture that will be scheduled when we meet in 2 weeks.


### Cool Kaggle Kernel
---
I just came across this awesome [kaggle kernel](https://www.kaggle.com/cdelany7/exploration-of-college-salaries-by-major#) analyzing some data about salaries by undergraduate major. The author does an awesome job of creating a cool visualization in steps. Check it out!

### Lecture 9
---
Our focus this week was on examining relationships between two variables. Scatter plots are visualizations used to examine the relationship between 2 numerical features. We spoke about ways of improving scatter plots when working with larger datasets and then discussed correlation statistics as ways of quantifying the strength of relationships between variables. Remember that Pearsons-moment correlation quantifies the strength of a **linear** relationship between variables. A correlation of 0 does not necessarily mean no relationship, but it does mean no linear relationship. We then spent a fair amount of time applying these concepts to the Austin bikeshare dataset. Here is that [notebook](https://github.com/lpatruno/stats-fall17/blob/master/notebooks/Lecture%209%20-%20Scatter%20Plots%20%26%20Correlation.ipynb).

Your homework assignment for next class is as follows:

  1. Read Ch. 8 of ThinkStats2 and run through the code in the chapter. This chapter is about estimation - the practice of estimating quantities that describe a population from finite samples. You'll encounter several extremely important concepts including standard error, sampling bias, confidence intervals, and sampling distributions.


### Lecture 8
---
This week we spent the class reviewing midterm project submissions. It was a great chance to learn from your peers, ask one another questions, and find out about difficulties encountered during your work. Nice job, everyone!

Your homework assignment for next class is as follows:

  1. Read Ch. 7 of ThinkStats2 and run through the code in the chapter. This chapter begins our foray into looking at relationships among different variables in your dataset. Although I won't ask you to hand this in, it's a good idea to begin applying these methods to your own datasets, even if you don't fully understand the concepts. We'll review the concepts more in class.
  
  2. Check out this awesome [visual intro to machine learning](http://www.r2d3.us/visual-intro-to-machine-learning-part-1/). Amazing visualizations! This is a great example of using technology to improve education! Also, I just came across this awesome collection of [cheat sheets](https://medium.com/towards-data-science/collecting-data-science-cheat-sheets-d2cdff092855) for data analysis in Python. Definitely check these out! There are cheat sheets for pandas, amtplotlib, seaborn, and more. Great resource.

### Map Visualizations
---
Several students have asked about how to visualize geographic information by creating maps. Arguably the best tools for visualizaing geographic information are written in JavaScript. [D3](https://d3js.org/) is one of the finer tools for this and the author of the library has written a series of [tutorials](https://medium.com/@mbostock/command-line-cartography-part-1-897aa8f8ca2c) for creating beautiful maps. I encourage you to check them out!

### Lecture 7
---
This week we concluded the first half of our semester by discussing probability density functions and kernel density estimation. Probability Density Functions, or PDFs, allow us to define probability distributions for continuous random variables. The PDF is the derivative of the Cumulative Distribution Function. Evaluating the PDF at a particular point does not give us the probability of that value occuring; rather, it gives us a probability density. In order to compute a probability, we need to integrate the PDF over some range i.e. compute the area underneath the curve. We showed in class how probability mass functions, cumulative distribution functions, and probability density functions are all related.

We also discussed kernel density estimation (KDE). KDE is a nonparametric way of computing a smooth distribution that fits a finite sample of data. This is useful for visualization, interpolation, and simulation, and an alternative method to model data.

Your homework assignment for next class is as follows:

  1. Your midterm projects are due by next class! Please see the directions [here](midterm_rubric.pdf) to remind yourself of what is expected. Be prepared to discuss these projects in class with your classmates.

### Lecture 6
---
Our class this week was on modeling empirical distributions with analytic distributions. Analytic distributions are characterized by a cumulative distribution function that is a mathematical function. Modeling empirical data with analytic distributions is useful if the models capture relevant aspects of the real world and leave out unneccessary details such as measurement error or specific quirks from a sample. Models also act as a form of data compression, allowing us to summarize large amounts of data with a small set of parameters.

We spoke specifically about the [exponential](https://en.wikipedia.org/wiki/Exponential_distribution), [normal](https://en.wikipedia.org/wiki/Normal_distribution), [lognormal](https://en.wikipedia.org/wiki/Log-normal_distribution), and [pareto](https://en.wikipedia.org/wiki/Pareto_distribution) distributions. I would highly recommend reading through the links provided to get a better understanding of the types of real-world phenomena that these distributions model. We also spoke about the types of transformations and plots we can create to determine whether or not these distributions fit out data well. For instance, to determine if data can be approximated by a normal distribution, we plot a normal probability plot and examine whether the plot is linear. Check out this week's [notebook](notebooks/Lecture%206.ipynb) where I used these tests to model data from the Austin bikeshare dataset.

Your homework assignment for next class is as follows:

  1. Read Ch. 6 of ThinkStats2. This chapter is on probability density functions, which describes the relative likelihood for a continuous variable to take on a given value. This chapter ties together the previously seen concepts of probability mass functions (PMFs) and cumulative distribution functions (CDFs) and concludes the introductory material of the class. Running through the code is not optional. It is a mandatory part of the assignment.
  
  2. Keep working on your midterm projects. They're due in 2 weeks on October 24th!
  
  3. A student mentioned the concept of the [bootstrap](https://en.wikipedia.org/wiki/Bootstrapping_(statistics)) in class yesterday. Bootstrapping is a method for estimating some property of an estimator by measuring those properties from some approximating distribution, often times the empirical distribution. Essentially, we resample the empirical distribution with replacement and compute some statistic, such as the variance. We will learn much more about estimation in chapter 8 of the text.

As always, email me with any questions!

### Lecture 5
---
This week we focused on Cumulative Distribution Functions - functions that map from values to percentiles. First, we noted that we run into issues when plotting histograms for variables that contain many different values. Namely, histograms will be hard to interpret because it will be difficult to see the overall pattern. One way of getting around this is to discretize or *bin* our data. However, we are then tasked with picking appropriate bin sizes, which is not trivial. In order to pick bin sizes, data analysts typically try a range of bin sizes through trial-and-error (we mentioned more [principled techniques](http://docs.astropy.org/en/stable/visualization/histogram.html) in class).

A better way to deal with this issue is to plot the CDF, which provides an informative visual representation of the shape of a distribution. Common values appear as steep or vertical sections of a CDF. If there are few values at a certain percentile, the CDF is flat in this range. CDFs are especially useful for comparing distributions, as plotting multiple CDFs on the same graph makes the shape of the distribution as well as differences more apparent. We generated some normally distributed test data and plotted the resulting CDF in [this week's notebook](notebooks/Lecture%205.ipynb).

Your homework assignment for next class is as follows:

  1. Read Ch. 5 of ThinkStats2. This is the most difficult material we will have encountered thus far. Pay particular attention to the author's description of how to determine if data is modeled by an analytic distribution. You will be required to use these methods in your projects. Please run through the code in the chapters. Running through the code is not optional. It is a mandatory part of the assignment.
  
  2. I've posted the [midterm rubric](midterm_rubric.pdf). Please refer to this document and ask me any questions you may have.

As always, email me with any questions!

### Lecture 4
---
This week we introduced the concept of probability mass functions (PMFs). Whereas histograms map from values to integer counts, PMFs map from values to probabilities. These can be visualized as bar graphs or hollow histograms and are useful for comparing multiple distributions since PMFs account for differences in sample size. In this weeks [Jupyter notebook](notebooks/Lecture%204.ipynb), I gave a few examples of using PMFs to compare different distributions found within the Austin bikeshare dataset.

Your homework assignment for next class is as follows:

  1. Read Ch. 4 of ThinkStats2. Please run through the code in the chapters. Running through the code is not optional. It is a mandatory part of the assignment.
  
  2. If I've emailed you asking for further clarification on your research questions, please email me back with the clarifications I've requested. By this point, you should all be working on your midterm projects, which are due on October 24th. I will follow up with additional details about the project. At a high level, I will expect a Jupyter notebook containing analysis similar to the analysis encountered so far in the textbooks.
  
As always, email me with any questions!

### Lecture 3
---
Yesterday we spent time speaking about different forms of exploratory data analysis. After discussing histograms, outliers, effect sizes, and summary statistics (and a few other things), we discussed a [Jupyter notebook](notebooks/Lecture%203.ipynb) I put together applying these ideas to an Austin bikeshare dataset. In that notebook I introduced a new Python library, [seaborn](https://seaborn.pydata.org/), which "provides a high-level interface for drawaing attractive statistical graphs." I recommend checking out some of the tutorials on the seaborn site, they're quite good.

Your homework assignment for next class is as follows:

  1. Read Ch. 3 of ThinkStats2. Please run through the code in the chapters.
  
  2. Read Ch. 2 of OpenStats except section 2.3.
  
As always, email me with any questions!

### Lecture 2
---
This past week we began to dig into practical techniques for analyzing data. 

First, we examined some useful ways of reading in and slicing through data using the Python package [pandas](http://pandas.pydata.org/pandas-docs/stable/). In order to demonstrate some of these techniques, I put together a simple Jupyter notebook, which you can access [here](notebooks/lecture_2.ipynb). If you click on the link, you'll see the Jupyter notebook rendered directly in the browser, as if you were running the notebook on your own machine. In order to actually run the cells, though, you'll have to clone the repo and run the notebook on your own machine. If you haven't used Github before, here is a short [interactive tutorial](https://try.github.io/levels/1/challenges/1).

We also spent some time examining a [**HarvardX	and	MITx: Four	Years	of	Open	Online	Courses**](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2889436), a statistical analysis of four years worth of data on the EdX MOOC platform. Specifically, we discussed the format of the paper and several of the visualizations. Note how the authors put forth several important questions, provide brief answers to these questions, and support these answers with carefully arranged descriptive statistics and well thought out data visualizations. Spend some time going through other visualizations within the document. Do you see the points the authors are trying to make? Do you think the authors' claims are well evidenced?

A few students mentioned difficulties with understanding the Python code. Allen Downey, the author of ThinkStats, has also written a textbook for learning Python 3 called [ThinkPython2e](http://greenteapress.com/wp/think-python-2e/). If you like the style of our textbook, I encourage you to check it out. Alternatively, check out this [interactive textbook](https://runestone.academy/runestone/static/thinkcspy/index.html). [Automate the Boring Stuff with python](https://automatetheboringstuff.com/) is also a fantastic resource for learning how to do some interesting things in Python, like [Sending Email and Text Messages](https://automatetheboringstuff.com/chapter16/).


Your homework assignment for next class is as follows:

  1. Read the Ch. 2 of ThinkStats2. Please run through the code in the chapters.
  
  2. If you haven't already done so, please read Ch. 1 of OpenStats. If you have read it, please skim through it again.
  
  3. Put together a proposal for your midterm and final project. I'd like you to propose *3* possible projects, each utilizing a different dataset. For each possible project, please include:
      * A guiding research question you seek to answer.
      * A dataset (or datasets) that you will analyze in order to answer the research question. If the dataset exists somewhere, please include a link to the dataset. If the dataset does not exist in a ready-to-use format, but you'd like to access data by writing a web scraper, polling an API, etc, please describe how you will do this.
      * A description of the variables within your dataset.
    
Please email me this proposal before the start of class next week. 

As always, email me with any questions!


### Lecture 1
---

Thank you for a very enjoyable discussion last night! I really enjoy teaching this course because of the way students are able to explore their interests through their personal projects. I'm looking forward to learning about a diverse range of topics through your projects!

As I mentioned in class, I will be using this site to post resources, links, lecture reviews, and homework assignments.

During our first lecture we spent time discussing the course [syllabus](Syllabus.pdf), including the grading breakdown for the course and the midterm and final projects. We also spent time reviewing some of the visualizations in this [Kaggle kernel](https://www.kaggle.com/benhamner/python-data-visualizations). Reviewing Kaggle kernels is a great way to learn about different applied data analysis methods and visualizations. 

Kaggle is also a great source of publically available [datasets](https://www.kaggle.com/datasets). This [Github repo](https://github.com/caesar0301/awesome-public-datasets) contains more datasets and [Amazon](https://aws.amazon.com/public-datasets/) and [Google](https://cloud.google.com/bigquery/public-data/) also host other datasets. I encourage each of you to look through these resource to find datasets for your term projects. Feel free to find other datasets or come up with your own by writing web scrapers. Here is a simple [tutorial](https://automatetheboringstuff.com/chapter11/) for how you might do that.


Your homework assignment for next class is as follows:

  1. Read the Preface and Chapter 1 of ThinkStats2. Please run through the code in the chapters. In order to do that you'll have to...
  
  2. Install [Anaconda](https://www.anaconda.com/download/) on your machines. We will be using Python 3.6 in this class.
  
  3. Work on exercise 1.3 in ThinkStats2. This asks you to think about a personal project. Part of your homework assignment for next class will be to submit a formal proposal for your midterm and final projects.
  
  4. Skim Chapter 1 of OpenStats. This chapter contains useful methods for performing exploratory data analysis of numerical and categorical data. You'll also get to read more about some of the visualizations we discussed in class yesterday.

If anyone has any questions, please feel free to email me!
