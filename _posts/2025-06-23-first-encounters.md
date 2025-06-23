---
title: "🕵️‍♀️ Inside the Mind of a Data Intern: First Encounters with Fraud Detection & ML"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - fraud detection
  - machine learning
  - internship
---

## The What and the Why

About a year ago, I was first introduced to the concept of machine learning. As part of my summer internship, I was brought on to develop a fraud detection model using purchase and sales data for the audit team. 
Having no prior experience in fraud detection, one of the first things I did— which you may have rightly guessed—was Google “fraud detection.”

According to the [Association of Certified Fraud Examiners](https://www.ibm.com/think/topics/fraud-detection), U.S. businesses lose 5%of their gross annual revenue to fraud. That 5% could fund new hires, equipment upgrades, or product innovations—instead, it quietly vanishes. That number fueled my why.

<!--more-->

## Figuring Out the How

Now that I had the what and why, I had to figure out the how.
As I dove deeper into fraud detection, I found that there are two main approaches organizations use: **rule-based systems** and **machine learning (ML) models**.
The rule-based method works just like it sounds, since it uses a set of predefined conditions to flag suspicious transactions. As explained in [Fraud.net’s glossary](https://www.fraud.net/glossary/rules-based-fraud-detection#what-is-rules-based-fraud-detection), 
these rules could include things like unusually high transaction amounts, odd timing, suspicious locations, or transaction frequency anomalies.
The second approach—machine learning—felt more mysterious and technically intimidating. However, the more I explored, the more I realized it didn’t have to be so abstract.

## Deconstructing Machine Learning (ML)
I’ve always pictured ML as a machine with a notepad clutched in its clunky metal hands, scribbling observations. In a way, that image isn’t too far off.

Machine learning is a process where computers learn from data by identifying patterns. According to a [Stripe article](https://stripe.com/resources/more/how-machine-learning-works-for-payment-fraud-detection-and-prevention), these patterns are used to help machines make decisions. 

In the case of fraud detection, an ML model can be trained on historical transaction data to learn what constitutes "normal" behavior—then flag transactions that deviate from those patterns.

## Selecting an Approach

Now came the question: which approach made the most sense for my project?

**Rule-based systems** are straightforward to implement and fast to execute. But they rely entirely on human-defined rules, making them rigid. They can miss novel fraud patterns that don’t fit the existing rule set. It also requires human intervention to keep updating the rules. Also, fraudsters may find ways to bypass these rules.

**Machine learning models**, on the other hand, don’t require hand-crafted rules. They can identify subtle, complex patterns from the data itself. This makes them adaptive and scalable. As the [Mangopay blog](https://blog.mangopay.com/en/home/machine-learning-models-vs-rule-based-systems-in-fraud-prevention-0) explains, if new fraud methods evolve over time, the model can be retrained on new data to detect these emerging threats—without manually rewriting rules.

That said, ML models can be harder to interpret. While you can usually explain why a rule flagged a transaction, ML models may act as black boxes: the inputs and outputs are clear, but the decision-making process in between can be opaque.
For this project, scalability and holistic approach was key. Instead of missing potential blind spots with the rule-based approach, I selected the ML approach!

## End-of-Day Notes
As I wrapped up my first few days of research, some of the next steps that I had jotted in my notebook included:

- Which fraud detection model should I select?
- How can I plan quick test runs?
- What types of ML models are best suited for this problem?
- What math is involved? (for my geeky side 😀)

### P.S.
I'll dive into these questions and the technical next steps in my next blog post—stay tuned!

## Sources

1. [IBM Think](https://www.ibm.com/think/topics/fraud-detection)  
2. [Fraud.net Glossary](https://www.fraud.net/glossary/rules-based-fraud-detection#what-is-rules-based-fraud-detection)  
3. [Stripe on ML for Fraud](https://stripe.com/resources/more/how-machine-learning-works-for-payment-fraud-detection-and-prevention)  
4. [Mangopay Blog](https://blog.mangopay.com/en/home/machine-learning-models-vs-rule-based-systems-in-fraud-prevention-0)
