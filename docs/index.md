---
layout: default
title: Home
header: Machine Learning from Time Series
nav_order: 1
---

## Overview

Time series machine learning is a rapidly evolving field that finds areas of application in all domains of machine learning and data science. This tutorial will provide an accessible overview of the recent research in a range of time series tasks, including classification, regression, clustering, anomaly detection, segmentation and similarity search. This is a wide ranging introduction to a multitude of research fields. These primers are not meant to be definitive: we could provide a tutorial on each topic in isolation. However, our goal is to raise awareness of the whole research field of time series machine learning and highlight the new and exciting work occurring in each area. Alongside describing tasks and algorithms, we will provide practical examples and comparisons using the [_aeon_](https://www.aeon-toolkit.org) toolkit, an open source, [_scikit-learn_](https://scikit-learn.org/) compatible framework for time series machine learning.

## When & Where

- Conference: [ECML 2024](https://ecmlpkdd.org/2024/)
- Date: Monday, September 09
- Time: 14:00 - 18:00 
- Room: Zeta 2

## Prerequisites

This tutorial is aimed at those interested in the basics of time series machine learning research.

- Basic machine learning background
- For code examples: Basic understanding of programming in Python and/or Jupyter notebooks 
- Not required code examples but helpful: Basic understanding of the _scikit-learn_ Python package

## Background

This is a broad overview tutorial aimed at highlighting the large body of recent research into Time Series Machine Learning (TSML) and encouraging the use of these algorithms when presented with time series data. Throughout the talk, we will use [_aeon_](https://www.aeon-toolkit.org) \[[1](https://doi.org/10.48550/arXiv.2406.14231)\] as a means of delivering practical examples for some of the algorithms that we introduce. We aim to demonstrate that these approaches are both effective and easily accessible for researchers.  

In the beginning of the tutorial we present an overview of recent time series research in the classic machine learning research fields of classification, regression and clustering with practical demonstrations. Next we introduce time series specific learning tasks: similarity search, segmentation and anomaly detection. We include a session dedicated to deep learning machine learning research, highlighting advances in all previously covered tasks. We do not address time series forecasting, since it was covered in depth in a [2023 ECML tutorial](https://lovvge.github.io/Forecasting-Tutorial-ECML-2023/) and we are limited in time and topics. 

Time series classification (TSC) \[[2](https://doi.org/10.1007/s10618-016-0483-9),[3](https://doi.org/10.1007/s10618-024-01022-1)\] involves fitting a model from a continuous, ordered sequence of real valued observations (a time series) to a discrete response variable. Time series extrinsic regression (TSER) \[[4](https://doi.org/10.1007/s10618-021-00745-9),[5](https://doi.org/10.1007/s10618-024-01027-w)\] uses a continuous response variable. Time series can be univariate (a single variable observed at each time point) or multivariate (multiple variables observed at each time point). TSC and TSER problems come from various domains, including medical signals such as ECG and EEG; HAR and other motion data; spectrograms; audio; electricity usage; and many more with industrial and academic applications. In the tutorial, we will highlight how we learn from time series data using the latest techniques, and why these techniques are preferable to more traditional machine learning approaches.

Time series clustering (TSCL) is the act of grouping time series data without recourse to a label. Algorithms that cluster time series can be classified into two groups: those that employ a time series specific distance measure, and those that derive features from time series. _aeon_ contains a range of distance based and feature based TSCL algorithms. We will focus primarily on distance based approaches \[[6](https://doi.org/10.1007/s10115-023-01952-0)\] and show how many widely held beliefs about distance based clustering are not supported by experimental evidence.

Similarity search consists in exploring a space of objects given as comparator the similarity between pairs of objects. In a time series context, these objects can be defined as time series or time series subsequences, and the comparator as a similarity function between two time series. Similarity search is used by many machine learning algorithms, for example in a _K_-NN, a time series to classify would be defined as a query, and the space of objects as the time series database. We then want to answer the query by searching for the _K_ most similar time series in the database. Performing similarity search also allows us to extract valuable information from the data, such as anomalies, repeating patterns or event precursors. As a field, one of the goals of similarity search is to provide efficient algorithms to explore large search spaces in a reasonable time. These algorithms can then be transposed to other machine learning algorithms relying on similarity search, such as shapelets, to also improve their efficiency. Another less obvious goal is to build estimators based on similarity search, which allows to leverage their efficiency and interpretability in some specific learning context, such as streaming data.

The study of natural and human-made processes often yields extensive sequences of time series data. These processes frequently exhibit multiple states, such as the operational modes of a machine, wherein transitions between states correspond to shifts in the distribution or shape of measured values. Time series segmentation (TSS) endeavours to detect these transitions post-hoc, thereby inferring changes in the underlying data-generating process. TSS is typically framed as an unsupervised learning problem aimed at identifying segments characterised by distinct statistical properties. While numerous TSS algorithms have been proposed \[[10](https://doi.org/10.1016/j.sigpro.2019.107299),[11](https://doi.org/10.1007/978-3-031-49896-1_1)\], many are tailored to specific domains. Conversely, only a handful of domain-agnostic TSS algorithms are available. We will spotlight state-of-the-art domain-agnostic segmentation algorithms and scrutinise advantages and limitations.

The task of anomaly detection consists of identifying rare or abnormal data deviating from normal or expected behaviour. In the context of time series, the task becomes even more challenging, given the multifactorial origins of anomalies. It is further complicated by the pervasive influence of noisy data, and the inherent seasonality and dynamism of real-world systems, which present formidable obstacles to effective anomaly detection. We will present some methods available in _aeon_ to tackle these challenges, which are based on a comprehensive evaluation \[[12](https://doi.org/10.14778/3538598.3538602)\].

Deep learning has shown a significant impact in both image and natural language processing domains. In 2019, it was shown that deep learning models can achieve state of the art performance for Time Series Classification \[[7](https://doi.org/10.1007/s10618-019-00619-1)\]. Subsequent research lead to the development of InceptionTime and its variants. Shifting the topic to deep clustering, another review in 2022 \[[8](https://doi.org/10.1007/s10618-021-00796-y)\] showed that deep learning architectures can be helpful in the case of clustering where the deep learning model's goal is to learn a compact self representation of the input space. Self representation learning \[[9](https://doi.org/10.5220/0011611300003393)\] is an unsupervised deep learning task with a goal of training a model to find a compact representation of time series that can be useful to following tasks, such as fine tuning. In the case where data are labelled with continuous values in terms of extrinsic regression tasks, any of the deep learning models proposed for classification can be simply adapted to regression tasks by changing the last layer's behaviour. We will focus on the different deep learning architectures that have been proposed for time series tasks, with extra attention for classification, clustering and regression.

## References 


[[1]](https://doi.org/10.48550/arXiv.2406.14231)  __Matthew Middlehurst__, __Ali Ismail-Fawaz__, __Antoine Guillaume__, Christopher Holder, __David Guijo Rubio__, Guzal Bulatova, Leonidas Tsaprounis, Lukasz Mentel, Martin Walter, __Patrick Schäfer__, __Anthony Bagnall__. aeon: a Python toolkit for learning from time series. arXiv preprint arXiv:2406.14231, 2024.

[[2]](https://doi.org/10.1007/s10618-016-0483-9) __Anthony Bagnall__, Jason Lines, Aaron Bostrom, James Large, and Eamonn Keogh. The great time series classification bake off: a review and experimental evaluation of recent algorithmic advances. Data Mining and Knowledge Discovery, 31(3):606–660, 2017.

[[3]](https://doi.org/10.1007/s10618-024-01022-1) __Matthew Middlehurst__, __Patrick Schäfer__, and __Anthony Bagnall__. Bake off redux: a review and experimental evaluation of recent time series classification algorithms. Data Mining and Knowledge Discovery, 1-74, 2024.

[[4]](https://doi.org/10.1007/s10618-021-00745-9) Chang Wei Tan, Christoph Bergmeir, Francois Petitjean, and Geoffrey Webb. Time series extrinsic regression. Data Mining and Knowledge Discovery, 35:1032––1060, 2021.

[[5]](https://doi.org/10.1007/s10618-024-01027-w) __David Guijo-Rubio__, __Matthew Middlehurst__, Guilherme Arcencio, Diego Furtado Silva, and __Anthony Bagnall__. Unsupervised feature based algorithms for time series extrinsic regression. Data Mining and Knowledge Discovery, 1-45, 2023.

[[6]](https://doi.org/10.1007/s10115-023-01952-0) Christopher Holder, __Matthew Middlehurst__, and __Anthony Bagnall__. A review and evaluation of elastic distance functions for time series clustering. Knowledge and Information Systems, 2023.

[[7]](https://doi.org/10.1007/s10618-019-00619-1) Hassan Ismail Fawaz, __Germain Forestier__, Jonathan Weber, Lhassane Idoumghar, and Pierre-Alain Muller. Deep learning for time series classification: a review. Data Mining and Knowledge Discovery, 33(4):917–963, 2019.

[[8]](https://doi.org/10.1007/s10618-021-00796-y) Baptiste Lafabregue, Jonathan Weber, Pierre Gancarski, and __Germain Forestier__. End-to-end deep representation learning for time series clustering: a comparative study. Data Mining and Knowledge Discovery, 36:29—-81, 2022.

[[9]](https://doi.org/10.5220/0011611300003393) __Ali Ismail-Fawaz__, Maxime Devanne, Jonathan Weber, and __Germain Forestier__. Enhancing time series classification with self-supervised learning. In Proceedings of the 15th International Conference on Agents and Artificial Intelligence - Volume 3: ICAART, pages 40–47. INSTICC, SciTePress, 2023.

[[10]](https://doi.org/10.1016/j.sigpro.2019.107299) Charles Truong, Laurent Oudre, and Nicolas Vayatis. Selective review of offline change point detection methods. Signal Processing, 167:107299, 2020.

[[11]](https://doi.org/10.1007/978-3-031-49896-1_1) __Arik Ermshaus__, __Patrick Schäfer__, __Anthony Bagnall__, Thomas Guyet, Georgiana Ifrim, Vincent Lemaire, Ulf Leser, Colin Leverger, and Simon Malinowski. Human Activity Segmentation Challenge - Discovery Challenge @ECML/PKDD’23. In International Workshop on Advanced Analytics and Learning on Temporal Data, pages 3–13. Springer, 2023.

[[12]](https://doi.org/10.14778/3538598.3538602) __Sebastian Schmidl__, __Phillip Wenig__, and __Thorsten Papenbrock__. Anomaly Detection in Time Series: A Comprehensive Evaluation. Proceedings of the VLDB Endowment (PVLDB), 15(9):1779–1797, 2022.
