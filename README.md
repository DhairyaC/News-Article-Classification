## Overview

## Goal

## Objectives
1. Perform web scraping to extract data (Business and News articles) from News API. It should contain at least 1000 words in total and at least two categories with at least 100 examples per category.
2. Split the dataset into training (at least 160 examples) and test (at least 40 examples) sets.
3. Fine-tune a pretrained language model (Albert-base-v2) capable of generating text on this dataset (the one I created in part 1). Report the test accuracy. Discuss what could be done to improve accuracy.
4. Try a couple of different language models (GPT-J and GPT-Sw3) to gain a better understanding.

## Techniques/Models
1. Techniques:
   - Web Scraping
   - Tokenization
   - Model optimization
   - Performance evaluation
2. Models:
   - Albert-base-v2 (a pre-trained model for sequence classification from Hugging Face Transformers)
   - GPT-J
   - GPT-Sw3

## Findings
1. After training the Albert-base-v2 model with 20 epochs, we observe a decrease in the training loss at each step. The accuracy obtained was 85%, which is higher than the accuracy obtained with 4 epochs. However, we could have achieved even higher accuracy if we had used a larger model or added regularization techniques like dropout to prevent overfitting. We could further experiment different batch sizes. A smaller batch size may allow the model to generalize better.
2. GPT-J is computationally expensive since the model requires around 24.2 GB of memory space to download. It is too big to be used on regular hardware: wouldn’t fit in RAM.
3. GPT-Sw3 is not released publicly: requires token access.
