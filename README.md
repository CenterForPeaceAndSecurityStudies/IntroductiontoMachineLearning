# Introduction to Machine Learning

This is a 6 hour introduction to machine learning spread across two three-hour lectures. The goal of this short course is very specific: to give you enough of an overview, vocabulary, and intuition, so that you can identify machine learning problems in the wild and begin your own research into relevant literatures and possible approaches. The goal is not to train you to execute a particular machine learning solution. There are far too many approaches available; they may not cover whatever problem you find; and the state of the art will be different in a year or two anyway. Instead, we will learn how to think about and classify problems into broad types, how to define and measure the efficacy of different solutions to that problem, how to avoid some common and subtle mistakes, and how to think about a full machine learning pipeline from start to finish.

# Readings Policy
Math and programming is not something you learn, it's something you get used to. It is a trade, that takes years of trial and error and concrete projects to acquire. The readings and assignments of this course are with minor exception voluntary and intended for self study. They are to help point you in the right direction when you realize you need to start brushing up on a particular set of tools in order to tackle a particular problem.

# Preliminiaries

## Software and Programming
Students are not expected to know any particular language or set of software. We will be demonstrating best practices as used in the Machine Learning for Social Science Lab at the Center for Peace and Security Studies, UCSD. In that lab, our software stack consists of Python and R for data preparation and analysis, Spark for database management, Keras/Tensorflow for deep learning, Github for revision control, and Ubuntu for our operating system and commandline tools.

Optional Readings
MACS 305001 - Computing for the Social Sciences, Benjamin Soltoff, Lecturer in Computational Social Science,
https://cfss.uchicago.edu/index.html

"R for Data Science", Garrett Grolemund, http://r4ds.had.co.nz/

"Spark and sparklyr," https://cfss.uchicago.edu/distrib003_spark.html

"GitHub and RStudio," https://resources.github.com/articles/github-and-rstudio/

Jeroen Janssens, "Data Science at the Command Line," February 8, 2018, https://www.datascienceatthecommandline.com/

Kieran Healy, "Data Visualization: A practical introduction", http://socviz.co/index.html?utm_content=buffer09710&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer

"Introduction to Validate," https://cran.r-project.org/web/packages/validate/vignettes/introduction.html

Thomas Nield, "An introduction to regular expressions," December 13, 2017 , https://www.oreilly.com/ideas/an-introduction-to-regular-expressions

RegExplain, "https://github.com/gadenbuie/regexplain/#readme"

Kieran Healy, "The Plain Person’s Guide to Plain Text Social Science," 2018-04-28, http://plain-text.co/


# Day 1
Course Slides: https://docs.google.com/presentation/d/19i2om_jwK8m3a-jNvgtM-WMT1l1HAGaGuWeb4bgLsTM/edit?usp=sharing

## Big Picture: What is our main job in machine learning? (What exactly is it that we doooo here?)

Readings
Leo Breiman, "Statistical Modeling: The Two Cultures (with comments and a rejoinder by the author)," Statistical Science, 2001, Vol. 16, No. 3, 199–231, https://projecteuclid.org/download/pdf_1/euclid.ss/1009213726


We explain them as parsimonously as possible as a function of other things.

Christopher Olah, "Visual Information Theory," October 14, 2015, http://colah.github.io/posts/2015-09-Visual-Information/

## Outcomes

## Distance

## Units of Analysis/Structure

## Features

## Models



## Information Theory
Christopher Olah, "Visual Information Theory," October 14, 2015, http://colah.github.io/posts/2015-09-Visual-Information/
C. E. SHANNON, "A Mathematical Theory of Communication," October 1948,  The Bell System Technical Journal, Vol. 27, pp. 379–423, 623–656, July,  http://math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf

Package ‘entropy,’ "Estimation of Entropy, Mutual Information and Related Quantities," February 19, 2015, http://strimmerlab.org/software/entropy/

Drost, (2018). Philentropy: Information Theory and Distance Quantification with R. Journal of Open Source Software, 3(26), 765, https://doi.org/10.21105/joss.00765

## What don't we do? (What isn't machine learning?)

### Causal Inference
Joshua D. Angrist & Jörn-Steffen Pischke, "Mostly Harmless Econometrics An Empiricist's Companion," 2009

Donald B. Rubin, "Basic Concepts of Statistical Inference for Causal Effects in Experiments and Observational Studies," 2004, 
http://www.stat.columbia.edu/~cook/qr33.pdf

## Sequences

Christopher Olah, "Understanding LSTM Networks," August 27, 2015, http://colah.github.io/posts/2015-08-Understanding-LSTMs/

Patrik Lindenfors, Fredrik Jansson, Yi-ting Wang and Staffan I. Lindberg, Christian Lopez, 05 March 2018, "Investigating Sequences in Ordinal Data: A New Approach With Adapted Evolutionary Models," https://www.cambridge.org/core/journals/political-science-research-and-methods/article/investigating-sequences-in-ordinal-data-a-new-approach-with-adapted-evolutionary-models/F3747D8A1908902BA7F26C5EE28AFAEF

# Day 2

 "Unsupervised Machine Learning: The hclust, pvclust, cluster, mclust, and more," https://quantdev.ssri.psu.edu/sites/qdev/files/Unsupervised_Machine_Learning_The_mclust_Package_and_others.html


#Feature Selection

"bounceR", R Package, https://github.com/STATWORX/bounceR

#Feature Reduction

#Feature Engineering


# Out of Sample

Interaction

Depth

Curse of Dimensionality



## Text
Julia Silge and David Robinson, "Text Mining with R: A Tidy Approach," 2018-04-02, https://www.tidytextmining.com/

"Introducing Monte Carlo Methods with R," https://www.slideshare.net/xianblog/introducing-monte-carlo-methods-with-r

Matthew Gentzkow, Bryan T. Kelly, Matt Taddy, "Text as Data," http://web.stanford.edu/~gentzkow/research/text-as-data.pdf



Terence Parr and Jeremy Howard, "How to explain gradient boosting," http://explained.ai/gradient-boosting/index.html


# Interpretation



# Causality

"When and How Should One Use Deep Learning for Causal Effect Inference", https://technionmail-my.sharepoint.com/personal/urishalit_technion_ac_il/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Furishalit_technion_ac_il%2FDocuments%2FPresentations%2FIAS2018%2FIAS2018_2_for_public%2Epdf&parent=%2Fpersonal%2Furishalit_technion_ac_il%2FDocuments%2FPresentations%2FIAS2018&slrid=aaa2759e-909e-5000-fd16-3e33cabf926f

Luke Keele, Dylan Small, "Comparing Covariate Prioritization via Matching to Machine Learning Methods for Causal Inference using Five Empirical Applications," May 11, 2018, https://arxiv.org/pdf/1805.03743.pdf

# Applications

Conflict forecasting
"ViEWS: a political Violence Early-Warning System," http://pcr.uu.se/research/views/

Michael Höhle, "Safe Disposal of Unexploded WWII Bombs," May 25, 2018, http://staff.math.su.se/hoehle/blog/2018/05/25/uxb.html

Infering Demographic Traits

Gaurav Sood and Suriyan Laohaprapanon, "Predicting Race and Ethnicity From the Sequence of Characters in a Name," May 8, 2018,  https://arxiv.org/pdf/1805.02109.pdf  
"ethnicolr: Predict Race and Ethnicity From Name," https://github.com/appeler/ethnicolr

# Interaction Terms

Jens Hainmueller Jonathan Mummolo Yiqing Xu, "How Much Should We Trust Estimates from Multiplicative Interaction Models? Simple Tools to Improve Empirical Practice," April 20, 2018, http://yiqingxu.org/papers/english/2018_HMX_interaction/main.pdf

## Installation

You can install the released version of IntroductiontoMachineLearning from [CRAN](https://CRAN.R-project.org) with:

``` r
install.packages("IntroductiontoMachineLearning")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
## basic example code
```

