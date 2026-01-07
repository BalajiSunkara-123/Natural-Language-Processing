# Natural Language Processing (CS374)

## Overview
This repository contains implementations of various **Natural Language Processing (NLP) models and algorithms** developed as part of the **CS374 – Natural Language Processing** course.

Each model is implemented independently to understand core NLP concepts using classical and statistical approaches.

---

## Implemented Models

### 1. 5-Gram Language Model (Author Style Text Generation)
- **Status:** ✅ Completed
- **Technique:** N-gram Language Model (n = 5)
- **Decoding Strategy:** Maximum Likelihood (Highest Probability Selection)
- **Author Used:** Arthur Conan Doyle
- **Dataset Source:** Project Gutenberg

This model generates text in the style of the selected author by predicting the next word based on the previous four words.

📂 Location:
N-Gram Model/
├── N-Gram Model.ipynb
├── data/
│ └── sherlock_holmes_corpus.txt

---

## Dataset Information
- Literary datasets are sourced from **Project Gutenberg**
- Texts are used in **plain text format (.txt)**
- Preprocessing steps include:
  - Removal of Project Gutenberg headers and footers
  - Conversion to lowercase
  - Whitespace normalization
  - Retention of punctuation to preserve writing style

---

## Model Details: 5-Gram Language Model

- **Tokenization:** Word-level with punctuation
- **Context Size:** 4 words
- **Probability Estimation:** Maximum Likelihood Estimation (MLE)

\[
P(w_5 | w_1, w_2, w_3, w_4) =
\frac{count(w_1, w_2, w_3, w_4, w_5)}
{count(w_1, w_2, w_3, w_4)}
\]

- The next word is selected using **argmax probability decoding**.

---

## Sample Outputs
The model was tested using seed sentences such as:
- *"holmes looked at me"*
- *"i could not believe"*
- *"the day was very cold"*

The generated text reflects the narrative style of Arthur Conan Doyle.

---

## How to Run
1. Navigate to the required model folder.
2. Open the Jupyter Notebook:
3. Run all cells sequentially.
4. Modify the seed text to generate new outputs.

---

## Limitations
- N-gram models do not capture long-range dependencies
- Deterministic decoding may lead to repetitive text
- No smoothing techniques applied

---

## Course Information
- **Course:** CS374 – Natural Language Processing  
- **Semester:** VI  
- **Institution:** National Institute of Technology, Andhra Pradesh (NIT AP)
- 3. Run all cells sequentially.
4. Modify the seed text to generate new outputs.

---

## Planned / Upcoming Models
- Bigram and Trigram Language Models
- Hidden Markov Models (HMM)
- Part-of-Speech Tagging
- Word Embeddings
- Text Classification Models

---

## Limitations
- N-gram models do not capture long-range dependencies
- Deterministic decoding may lead to repetitive text
- No smoothing techniques applied

---

## Course Information
- **Course:** CS374 – Natural Language Processing  
- **Semester:** VI  
- **Institution:** National Institute of Technology, Andhra Pradesh (NIT ANP)

