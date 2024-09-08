---
layout: default
title: Schedule
nav_order: 2
---

The tutorial is on __Monday, September 09__ starting at __14:00__ in room __Zeta 2__. The speakers will be available afterwards for Q&A, and questions are always welcome on the [_aeon_](/https://www.aeon-toolkit.org/) Slack (details on the website).

- Introduction to Time Series Machine Learning and _aeon_ - (14:00, 10 Minutes, by Anthony Bagnall)

  Special considerations must be given when it comes to processing and creating models from time series data. To begin we will be a brief overview of the time series data and the different kinds of time series data one may find. We will also briefly introduce the _aeon_ toolkit, which is used in our code examples.

  [Slides](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Slides/part1_introduction.pptx) & [Notebook (file)](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part1_introduction.ipynb) & [Notebook (Google Colab)](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part1_introduction.ipynb) 

- Classification and Regression - (14:10, 30 Minutes, by Matthew Middlehurst)

  Time series classification (TSC) and regression (TSER) are rapidly evolving fields that find areas of application in many domains.These will be among the more familiar tasks to those with knowledge of vector-based machine learning. We showcase the types of algorithms used for TSC and TSER, and how they learn from large variety of characteristics found in datasets of time series.

  [Slides](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Slides/part2_classification_regression.pptx) & [Notebook (file)](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part2_classification_regression.ipynb) & [Notebook (Google Colab)](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part2_classification_regression.ipynb)  

- Clustering - (14:40, 30 Minutes, by Anthony Bagnall)

  todo

  [Slides](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Slides/part3_clustering.pptx) & [Notebook (file)](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part3_clustering.ipynb) & [Notebook (Google Colab)](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part3_clustering.ipynb)  
  
- Similarity Search - (15:10, 20 Minutes, by Antoine Guillaume)

  Similarity search is a crucial task in time series machine learning, as any algorithm using a similarity measure might benefit from the computational improvements developed in this field. Particularly, algorithms based on sliding window operations, like shapelets, have a lot to gain from adopting similarity search methods. In this session, we will introduce three different tasks for similarity search, explain how they interact with each other, and present some example use cases. We'll showcase the improvements on computation time of some popular algorithms and talk about the future plans for this module in `aeon`.

  [Slides](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Slides/part4_similarity_search.pptx) & [Notebook (file)](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part4_similarity_search.ipynb) & [Notebook (Google Colab)](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part4_similarity_search.ipynb)   


- Segmentation - (15:30, 30 Minutes, by Arik Ermshaus and Patrick Schäfer)

  The study of natural and human-made processes often yields extensive sequences of time series data. These processes frequently exhibit multiple states, such as the operational modes of a machine, wherein transitions between states correspond to shifts in the distribution or shape of measured values. Time series segmentation (TSS) endeavours to detect these transitions post-hoc, thereby inferring changes in the underlying data-generating process. TSS is typically framed as an unsupervised learning problem aimed at identifying segments characterised by distinct statistical properties. While numerous TSS algorithms have been proposed, many are tailored to specific domains. Conversely, only a handful of domain-agnostic TSS algorithms are available. We will spotlight state-of-the-art domain-agnostic segmentation algorithms and scrutinise advantages and limitations.

  [Slides](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Slides/part5_segmentation.pptx) & [Notebook (file)](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part5_segmentation.ipynb) & [Notebook (Google Colab)](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part5_segmentation.ipynb)  

- Break (16:00, 30 Minutes)

- Anomaly Detection - (16:30, 30 Minutes, by Sebastian Schmidl)

  Time series anomaly detection is an important task in many domains, such as detecting structural defects in aircraft turbines, faulty states in water treatment plants, or anomalous heartbeats in healthcare monitoring. Researchers have developed numerous automatic methods to analyze and detect anomalous points and subsequences in time series data. However, many approaches are tailored to specific domains and there is no overall best domain-agnostic method. In this part of the tutorial, we will introduce the task of anomaly detection in time series data and give an overview of available anomaly detection methods and benchmarks.

  [Slides](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Slides/part6_anomaly_detection.pptx) & [Notebook (file)](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part6_anomaly_detection.ipynb) & [Notebook (Google Colab)](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part6_anomaly_detection.ipynb)   
  
- Deep learning - (17:00, 40 Minutes, by Ali Ismail-Fawaz)

  Deep learning is a subset of machine learning that uses multi-layer neural networks to automatically learn complex patterns in data. In time series tasks, it is applied to classification, clustering, regression, anomaly detection, and rapid prototyping. It is highly effective, as it can model complex temporal dependencies without requiring manual feature engineering, making it a powerful tool for time series analysis.

  [Slides](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Slides/part7_deep_learning.pdf) & [Notebook (file)](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part7_deep_learning_based.ipynb) & [Notebook (Google Colab)](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Notebooks/part7_deep_learning_based.ipynb)  

- Conclusion - (17:40, 10 Minutes, by Anthony Bagnall)

  TODO
  
  [Slides](https://github.com/aeon-toolkit/aeon-tutorials/blob/main/ECML-2024/Slides/part8_conclusion.pptx)

- Q&A (17:50, 10+ Minutes)
