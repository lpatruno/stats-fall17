## Welcome to CISC 5420 - Applied Statistics & Probability!

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
