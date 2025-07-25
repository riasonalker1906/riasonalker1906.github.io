---
title: "🕵️‍♀️ Inside the Mind of a Data Intern: Choosing My First ML Tools for Fraud Detection"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - fraud detection
  - machine learning
  - internship
related: false
comments: true
---

## Where I Last Left Off – Flipping Back To My E.O.D Notes
In my previous blog, I revisited the time as an intern, newly introduced to a fraud detection project. My early exploration involved scratching the surface of several new topics, including machine learning (ML), as I briefly outline the what, why and how behind this project. 

Flipping back to my End-Of-Day notes from that time, I was left with the over-arching question: **how can I apply ML to help achieve the project goal of detecting fraudulent transactions**?

<!--more-->

## Common ML Techniques in Fraud Detection

After the first few days of research into the basic concepts of ML, I began exploring how different models are used for detecting fraud. Here are a few key applications I noted:

- **Anomaly detection** – ML models are trained on historic data, such as regular and valid sales transactions, to understand what’s “normal” and identify unusual, potentially fraudulent, patterns.
- **Risk scoring** – Assigning a fraud-likelihood score to transactions based on factors like amount, frequency, or location.
- **Network analysis** – Analyzing relationships between entities (e.g., vendors, buyers) to identify suspicious links or behavior clusters.
- **Text analysis** – Examining textual data like messages or emails for keywords or patterns that suggest fraudulent intent.

## Narrowing Down ML Techniques for My Use Case

To determine which technique was suitable to test and experiment with for my project, I revisited its main objective: flagging potentially fraudulent purchase or sales transactions.

Given that I didn’t have labeled data readily available and needed a quick way to set up baseline models that flag abnormalities, anomaly detection seemed like a logical starting point.

## Anomaly Detection Model Lineup

Upon researching algorithms used for anomaly and fraud detection, I came across the following that could make good candidates to run initial tests on. Here’s who they are, and what they do:

- **One-Class Support Vector Machines (SVMs)** – These models train on data points from a single class (such as, legitimate transactions) and learn a boundary that defines “normal” behavior. Any data point falling outside this boundary is flagged as an anomaly.
- **Isolation Forest** – As explained by [scikit-learn’s User Guide](https://scikit-learn.org/stable/modules/outlier_detection.html), this is an ensemble of decision trees that isolates data points by randomly choosing features and split values. Since anomalies differ from normal data, they have shorter average path lengths, making them easy to isolate and detect.
- **K Nearest Neighbor (KNN)** – This method measures the average distance and finds the nearest neighbor for every data point. Points with the most significant distance from the population will be considered outliers.

## End-of-Day Notes

A sneak peek into notes I jotted after getting introduced to these techniques:

- **How do I evaluate these models—especially without labeled data?** Should I focus on proxy metrics like precision, false positive/negative rates (using synthetic labels), or prioritize practical aspects like scalability?
- **Any model assumptions I should be aware of?**

## Sources

1. [GeeksforGeeks – Types of Machine Learning](https://www.geeksforgeeks.org/machine-learning/types-of-machine-learning/)
2. [SQream – Fraud Detection with Machine Learning](https://sqream.com/blog/fraud-detection-machine-learning/)
3. [Stripe – How Machine Learning Works for Payment Fraud Detection](https://stripe.com/resources/more/how-machine-learning-works-for-payment-fraud-detection-and-prevention)
4. [Fraud.com – Anomaly Detection](https://www.fraud.com/post/anomaly-detection)
5. [Analytics Vidhya – One-Class SVM for Anomaly Detection](https://www.analyticsvidhya.com/blog/2024/03/one-class-svm-for-anomaly-detection/)
6. [scikit-learn – Outlier Detection](https://scikit-learn.org/stable/modules/outlier_detection.html)
7. [ScienceDirect – A Survey on Machine Learning Models for Fraud Detection](https://www.sciencedirect.com/science/article/pii/S2772662223000036#:~:text=The%20machine%20learning%20models%20of,model%20for%20predicting%20fraudulent%20transactions.)

