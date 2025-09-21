# NLPASSIGNMENT2
Name:Venkata Nanda Krishna Yaram.

st,id:700765514

This repository contains solutions for **Questions 1–8** from the NLP assignment. Each question involves theory, calculation, or coding tasks related to classification, evaluation, and language modeling.  

## **Q1 – Chain Rule of Probability**  
- The chain rule lets us express the probability of a sentence as a product of conditional probabilities.  
- Used in language modeling to break down \\( P(w_1, w_2, …, w_n) \\) into smaller terms.
 
## **Q2 – Naive Bayes Classification (Confusion Matrix)**  
- Computed **per-class Precision & Recall** for Cat, Dog, Rabbit.  
- Evaluated classifier performance using confusion matrix analysis.  
- Highlighted how metrics differ for each class.  

## **Q3 – Edit Distance**  
- Calculated **minimum edit distance** between two words under two models:  
  - Model A: Sub=1, Ins=1, Del=1.  
  - Model B: Sub=2, Ins=1, Del=1.  
- Wrote valid **edit sequence** step by step.  
- Computed partial **dynamic programming table** rows.  

## **Q4 – Harms of Classification**  
- **Representational Harm**: Reinforcing stereotypes (Kiritchenko & Mohammad, 2018).  
- **Censorship Risk**: Over-blocking of neutral identity-related content in toxicity systems.  
- **Varieties of English**: Worse performance on African American English or Indian English due to dataset bias.  

## **Q5 – Evaluation Metrics (Multi-Class Confusion Matrix)**  
- Computed **precision and recall** per class (Cat, Dog, Rabbit).  
- Calculated **macro-averaged** and **micro-averaged** metrics.  
- Explained interpretation:  
  - Macro = treats classes equally.  
  - Micro = weights by number of samples.  
- Included **Python implementation** for automation.  

## **Q6 – Bigram Probabilities & Zero-Probability Problem**  
- Computed MLE probabilities of:  
  - Sentence 1: `<s> I love NLP </s>`  
  - Sentence 2: `<s> I love deep learning </s>`  
- Compared which sentence is more probable.  
- **Zero-probability problem**: e.g., \\( P(\\text{noodle} \\mid ate) = 0 \\).  
- Solved with **Laplace smoothing (Add-1)** to avoid zeros.  

## **Q7 – Backoff Model**  
- Computed trigram-based \\( P(cats \\mid I, like) \\).  
- Used **trigram → bigram backoff** for \\( P(dogs \\mid You, like) \\).  
- Explained why **backoff** is essential to handle missing higher-order n-grams.  

## **Q8 – Programming: Bigram Language Model**  
- Implemented a **Bigram Language Model** in Python:  
  - Counted unigrams and bigrams.  
  - Estimated bigram probabilities using MLE.  
  - Built a function to compute sentence probability.  
- Tested on:  
  - `<s> I love NLP </s>`  
  - `<s> I love deep learning </s>`  
- The model prefers the sentence that appears more consistent with training data. 
