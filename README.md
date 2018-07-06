# Introduction to Machine Learning

Rex W. Douglass<br/>
Director Machine Learning for Social Science Lab (MSSL)<br/>
Center for Peace and Security Studies (cPASS)<br/>
Department of Political Science<br/>
University of California San Diego<br/>
rexdouglass@gmail.com<br/>
www.rexdouglass.com<br/>
@rexdouglass


## Overview

This is a 6 hour introduction to machine learning spread across two three-hour lectures. The goal of this very short course is specific: to give you enough of an overview, vocabulary, and intuition, so that you can identify machine learning problems in the wild and begin your own research into relevant literatures and possible approaches. The goal is not to train you to execute a particular machine learning solution. There are far too many approaches available; they may not cover whatever problem you find; and the state of the art will be different in a year or two anyway. Instead, we will learn how to think about and classify problems into broad types, how to define and measure the efficacy of different solutions to that problem, how to avoid some common and subtle mistakes, and how to think about a full machine learning pipeline from start to finish.

Day 1 is dedicated to providing intuition into the core ideas and problems in machine learning. The goal of the lecture will be to introduce those ideas using as simple of examples as possible. We will spend almost no time on specific tools, code, or real world examples.

Day 2 is dedicated almost entirely to tools and real world examples. We will grind through as many problems/solutions being used right now in three hours as we can, with links to further reading in the syllabus.

Please bring a two sided coin(s) and scratch paper to class for passing notes for the demonstrations.

### Readings Policy
Math and programming are not something you learn, they're something you get used to. It is a trade, that takes years of trial and error and concrete projects to acquire. The readings of this course are, with a few exceptions, voluntary and intended for self study. They are to help point you in the right direction when you realize you need to start brushing up on a particular set of tools in order to tackle a particular problem.

Required - Skim in order to improve discussion and understanding during lecture <br/>
Recommended - Eventually skim/read during self study <br/>
Reference - Deeper mathematical or historical context <br/>

### Textbooks

Do not purchase any books. Each of these should be available for free online at the link given.

(CIML)  [A course in machine learning](ciml.info/), Hal Daume III <br/>
(ESL) [Elements of Statistical Learning, Trevor Hastie(https://web.stanford.edu/~hastie/ElemStatLearn/), Robert Tibshirani <br/>
(ISL) [An introduction to statistical learning: with application in R, Gareth James](https://www-bcf.usc.edu/~gareth/ISL/ISLR%20Seventh%20Printing.pdf), Daniela Witten, Trevor Hastie, and Robert Tibshirani br/>
(IML) Introduction to Machine Learning[http://alex.smola.org/drafts/thebook.pdf], Alex Smola and S.V.N. Vishwanathan <br/>
(IMLR) ["An Introduction to Machine Learning with R"](https://lgatto.github.io/IntroMachineLearningWithR/index.html),Laurent Gatto, 2017-10-18 <br/>
(ML) [Machine Learning: The art and science of algorithms that make sense of data](http://dsd.future-lab.cn/members/2015nlp/Peter_Flach_Machine_Learning._The_Art_and_Scienc(BookZZ.org).pdf), Flach,  <br/>
(MLPP) [Machine Learning: A Probabilistic Perspective](https://www.cs.ubc.ca/~murphyk/MLbook/), Kevin Murphy, <br/>
(PRML) [Patter recognition and machine learning](http://users.isr.ist.utl.pt/~wurmd/Livros/school/Bishop%20-%20Pattern%20Recognition%20And%20Machine%20Learning%20-%20Springer%20%202006.pdf), Christopher M. Bishop <br/>
(WMLW) ["WHY MACHINE LEARNING WORKS"](http://www.cs.cmu.edu/~gmontane/montanez_dissertation.pdf), George D. Montanez, May 2017, Dissertation <br/>

### General Resources

There are a number places on-line for constant updates on machine learning
https://www.reddit.com/r/MachineLearning/<br/>
https://twitter.com/arxiv_org<br/>
https://twitter.com/RexDouglass<br/>
https://www.cambridge.org/core/journals/political-analysis<br/>


### Software and Programming

Students are not expected to know any particular language or set of software. We will be demonstrating best practices as used in the Machine Learning for Social Science Lab at the Center for Peace and Security Studies, UCSD. In that lab, our software stack consists of Python and R for data preparation and analysis, Spark for database management, Keras/Tensorflow for deep learning, Github for revision control, and Ubuntu for our operating system and command-line tools.

MACS 305001 - Computing for the Social Sciences, Benjamin Soltoff, Lecturer in Computational Social Science,
https://cfss.uchicago.edu/index.html <br/>
"R for Data Science", Garrett Grolemund, http://r4ds.had.co.nz/ <br/>
"Spark and sparklyr," https://cfss.uchicago.edu/distrib003_spark.html <br/>
"GitHub and RStudio," https://resources.github.com/articles/github-and-rstudio/ <br/>
Jeroen Janssens, "Data Science at the Command Line," February 8, 2018, https://www.datascienceatthecommandline.com/ <br/>
Kieran Healy, "Data Visualization: A practical introduction", http://socviz.co/index.html?utm_content=buffer09710&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer <br/>
"Introduction to Validate," https://cran.r-project.org/web/packages/validate/vignettes/introduction.html <br/>
Thomas Nield, "An introduction to regular expressions," December 13, 2017 , https://www.oreilly.com/ideas/an-introduction-to-regular-expressions <br/>
RegExplain, "https://github.com/gadenbuie/regexplain/#readme" <br/>
Kieran Healy, "The Plain Person’s Guide to Plain Text Social Science," 2018-04-28, http://plain-text.co/ <br/>
"Statistical Data Cleaning with Applications in R"

# Day 1 The Intuition
Course Slides: https://docs.google.com/presentation/d/19i2om_jwK8m3a-jNvgtM-WMT1l1HAGaGuWeb4bgLsTM/edit?usp=sharing

## Introduction

### What is machine learning?

(CIML), Chapter 1, http://ciml.info/dl/v0_99/ciml-v0_99-ch01.pdf

WMLW 1.0 "Introduction"

### What isn't machine learning?

#### Statistics

Leo Breiman, "Statistical Modeling: The Two Cultures (with comments and a rejoinder by the author)," Statistical Science, 2001, Vol. 16, No. 3, 199–231, https://projecteuclid.org/download/pdf_1/euclid.ss/1009213726

#### Causal Inference
Joshua D. Angrist & Jörn-Steffen Pischke, "Mostly Harmless Econometrics An Empiricist's Companion," 2009

Donald B. Rubin, "Basic Concepts of Statistical Inference for Causal Effects in Experiments and Observational Studies," 2004,
http://www.stat.columbia.edu/~cook/qr33.pdf


## Why Machine Learning

"ViEWS: a political Violence Early-Warning System," http://pcr.uu.se/research/views/

Michael Höhle, "Safe Disposal of Unexploded WWII Bombs," May 25, 2018, http://staff.math.su.se/hoehle/blog/2018/05/25/uxb.html

Gaurav Sood and Suriyan Laohaprapanon, "Predicting Race and Ethnicity From the Sequence of Characters in a Name," May 8, 2018,  https://arxiv.org/pdf/1805.02109.pdf  
"ethnicolr: Predict Race and Ethnicity From Name," https://github.com/appeler/ethnicolr

## Shannon–Weaver Model of Communication

https://en.wikipedia.org/wiki/Shannon%E2%80%93Weaver_model

Christopher Olah, "Visual Information Theory," October 14, 2015, http://colah.github.io/posts/2015-09-Visual-Information/

C. E. SHANNON, "A Mathematical Theory of Communication," October 1948,  The Bell System Technical Journal, Vol. 27, pp. 379–423, 623–656, July,  http://math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf

PRML 1.6 "Information Theory"

### Information Sources

### Entropy
https://en.wikipedia.org/wiki/Entropy_(information_theory)

### Distributions and Probability
Arian Maleki and Tom Do, "Review of Probability Theory," http://cs229.stanford.edu/section/cs229-prob.pdf

PRML 2.0

### Messages

### Transmitters
https://en.wikipedia.org/wiki/Function_(mathematics)

### Receivers
https://en.wikipedia.org/wiki/Inverse_function

# 0-bit information source

## 0-bit information source, 1-bit message
Zero information conversations

## 0-bit information source, 2-N bit message

# 1 bit information sources,

## Y vs Yhat

### Mutual information
https://en.wikipedia.org/wiki/Mutual_information

### Evaluating Reconstructions

https://en.wikipedia.org/wiki/Evaluation_of_binary_classifiers
https://en.wikipedia.org/wiki/Confusion_matrix
https://en.wikipedia.org/wiki/Precision_and_recall
https://en.wikipedia.org/wiki/Sensitivity_and_specificity
https://en.wikipedia.org/wiki/F1_score

### Distance and Similarity

Package ‘entropy,’ "Estimation of Entropy, Mutual Information and Related Quantities," February 19, 2015, http://strimmerlab.org/software/entropy/

Drost, (2018). Philentropy: Information Theory and Distance Quantification with R. Journal of Open Source Software, 3(26), 765, https://doi.org/10.21105/joss.00765

## 1 bit source, 1 bit messages

### What makes a good receiver?

PRML 1.5 "Decision Theory"

Scott Fortmann-Roe, "Understanding the Bias-Variance Tradeoff," 2012, http://scott.fortmann-roe.com/docs/BiasVariance.html

### No Free Lunch

WMLW 2.0 "Related Work"

"No Free Lunch Theorems for Optimization," David H. Wolpert and William G. Macready, 1997, https://ti.arc.nasa.gov/m/profile/dhw/papers/78.pdf

##Overfitting

### Parametric Receiver Function
#### Mean
#### Logit
https://en.wikipedia.org/wiki/Logistic_regression
#### SVM
https://en.wikipedia.org/wiki/Support_vector_machine

### In Sample/Out of Sample

https://en.wikipedia.org/wiki/Training,_test,_and_validation_sets
https://en.wikipedia.org/wiki/Cross-validation_(statistics)

### Cross Validation

"Linear Model Selection by Cross-Validation," Jun Shao, 1993, http://www.libpls.net/publication/MCCV_Shao_1993.pdf
"Cross-validation failure: small sample sizes lead to large error bars," Gaël Varoquaux, 2017, https://hal.inria.fr/hal-01545002/

## 1 bit information source, 2 bit message

### Features

#### Feature Engineering

https://en.wikipedia.org/wiki/Feature_engineering

### Interaction

https://en.wikipedia.org/wiki/Interaction_(statistics)

Jens Hainmueller Jonathan Mummolo Yiqing Xu, "How Much Should We Trust Estimates from Multiplicative Interaction Models? Simple Tools to Improve Empirical Practice," April 20, 2018, Political Analysis, http://yiqingxu.org/papers/english/2018_HMX_interaction/main.pdf

#### Dictionary Learning
https://en.wikipedia.org/wiki/Sparse_dictionary_learning

### Partioning

#### Nearest Neighbor
https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm

Integer encoder
Latent variable model

#### Clustering
https://en.wikipedia.org/wiki/Cluster_analysis

#### K-means
https://en.wikipedia.org/wiki/K-means_clustering


### Structure

#### Temporal

##### Sequences
Patrik Lindenfors, Fredrik Jansson, Yi-ting Wang and Staffan I. Lindberg, Christian Lopez, 05 March 2018, "Investigating Sequences in Ordinal Data: A New Approach With Adapted Evolutionary Models," https://www.cambridge.org/core/journals/political-science-research-and-methods/article/investigating-sequences-in-ordinal-data-a-new-approach-with-adapted-evolutionary-models/F3747D8A1908902BA7F26C5EE28AFAEF

#### Spatial
#### Network

## 2 bit information source, 1 bit message

### Bandwidth

### Over determination
https://en.wikipedia.org/wiki/Overdetermined_system

## 1-bit information source, N-bit message

### Curse of Dimensionality

https://en.wikipedia.org/wiki/Curse_of_dimensionality

####Feature Selection
https://en.wikipedia.org/wiki/Feature_selection

"bounceR", R Package, https://github.com/STATWORX/bounceR

P-Hacking
https://projects.fivethirtyeight.com/p-hacking/

## N-bit information source, 1-bit message

## 2 bit information source, 2 bit message

## N-bit information source, N-bit message
https://en.wikipedia.org/wiki/Binary_number#Counting_in_binary

## 1-bit information source, 1-bit message, 1-bit of line noise

# Day 2 The Toolbox

## Introduction

### Toy problems
UC Irvine Machine Learning Repository, http://archive.ics.uci.edu/ml/index.php

https://en.wikipedia.org/wiki/List_of_datasets_for_machine_learning_research

Kaggle Datasets, https://www.kaggle.com/datasets?sortBy=votes&group=all

https://projects.fivethirtyeight.com/2018-world-cup-predictions/

## Clustering

"Unsupervised Machine Learning: The hclust, pvclust, cluster, mclust, and more," https://quantdev.ssri.psu.edu/sites/qdev/files/Unsupervised_Machine_Learning_The_mclust_Package_and_others.html

## Non-parametric models

### Trees
https://en.wikipedia.org/wiki/Decision_tree_learning

### Ensembles
https://en.wikipedia.org/wiki/Random_forest

## Gradient Boosting
Terence Parr and Jeremy Howard, "How to explain gradient boosting," http://explained.ai/gradient-boosting/index.html

## Parametric Models

# OLS



https://en.wikipedia.org/wiki/Support_vector_machine

## Neural Networks

https://en.wikipedia.org/wiki/Artificial_neural_network

(DL) Deep Learning, Ian Goodfellow and Yoshua Bengio and Aaron Courville, 2016, http://www.deeplearningbook.org/

### LSTM
Christopher Olah, "Understanding LSTM Networks," August 27, 2015, http://colah.github.io/posts/2015-08-Understanding-LSTMs/

https://keras.rstudio.com/articles/examples/conv_lstm.html


## Text
Julia Silge and David Robinson, "Text Mining with R: A Tidy Approach," 2018-04-02, https://www.tidytextmining.com/

"Introducing Monte Carlo Methods with R," https://www.slideshare.net/xianblog/introducing-monte-carlo-methods-with-r

Matthew Gentzkow, Bryan T. Kelly, Matt Taddy, "Text as Data," http://web.stanford.edu/~gentzkow/research/text-as-data.pdf

## Images

https://keras.rstudio.com/articles/examples/cifar10_cnn.html

# Interpretation

"Why Should I Trust You?": Explaining the Predictions of Any Classifier, Marco Tulio Ribeiro, Sameer Singh, Carlos Guestrin, https://arxiv.org/abs/1602.04938

lime, Python Package, https://github.com/marcotcr/lime

# Causality

"When and How Should One Use Deep Learning for Causal Effect Inference", https://technionmail-my.sharepoint.com/personal/urishalit_technion_ac_il/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Furishalit_technion_ac_il%2FDocuments%2FPresentations%2FIAS2018%2FIAS2018_2_for_public%2Epdf&parent=%2Fpersonal%2Furishalit_technion_ac_il%2FDocuments%2FPresentations%2FIAS2018&slrid=aaa2759e-909e-5000-fd16-3e33cabf926f

Luke Keele, Dylan Small, "Comparing Covariate Prioritization via Matching to Machine Learning Methods for Causal Inference using Five Empirical Applications," May 11, 2018, https://arxiv.org/pdf/1805.03743.pdf
