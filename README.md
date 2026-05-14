# Vietnamese E-commerce Bag Review ABSA

Aspect-Based Sentiment Analysis (ABSA) and sentiment classification for Vietnamese e-commerce bag reviews collected from Tiki.

## Overview

This project focuses on two NLP tasks:

* **Overall Sentiment Classification**

  * Positive
  * Neutral
  * Negative

* **Aspect-Based Sentiment Analysis (ABSA)**

  * Aspect Detection
  * Aspect Sentiment Classification

The system analyzes user reviews for fashion bags and identifies sentiments associated with different product aspects such as quality, design, price, delivery, packaging, and size.

## Dataset

* Source: Tiki e-commerce platform
* Domain: Men's and women's fashion bags
* Language: Vietnamese

## Tech Stack

* Python
* scikit-learn
* PyTorch
* Hugging Face Transformers
* PhoBERT

## Models

### Baseline Models

* TF-IDF + Logistic Regression
* TF-IDF + SVM
* TF-IDF + Naive Bayes

### Transformer-based Models

* PhoBERT for Overall Sentiment Classification
* PhoBERT for Aspect Detection
* PhoBERT for Aspect Sentiment Classification

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-score
* Macro F1-score

## Project Structure

```text id="rxs7x3"
.
├── data/
├── docs/
├── notebooks/
├── reports/
├── src/
├── demo/
├── requirements.txt
└── README.md
```

## Example

Input:

```text id="p3px0x"
"Túi đẹp nhưng giao hàng hơi chậm"
```

Output:

```json id="rnz2n2"
{
  "overall_sentiment": "Neutral",
  "aspects": [
    {
      "aspect": "Design",
      "sentiment": "Positive"
    },
    {
      "aspect": "Delivery",
      "sentiment": "Negative"
    }
  ]
}
```
