# Question-answering-and-reading-comprehension-project
Question answering and reading comprehension project on the eHoVy RACE reading-comprehension dataset from Hugging Face. In this project, we train and compare a variety of deep learning models, especially large language models, to obtain information on smaller scale models and their generalization ability.

We begin with data loading and **preliminary analysis** to understand the structure, vocabulary and class balance of the dataset.

Next, we train and compare a variety of models:

1. **Simple baselines** (TF-IDF + logistic regression)  
2. **Sequence models** (LSTM-based classifier)  
3. **Large language model (LLM) zero-shot/feature-based** approaches  
4. **Fine-tuning an LLM** (flan T5) with Lora

Finally, we explore a few **extensions**:

- Applying our pipeline to **additional datasets** with the best fine-tuned ALBERT model
- Building a **distractor-generation model** to automatically craft plausible but incorrect answer choices  

> **Note:** For convenience, cells with all required `pip install` commands, imports and data-loading steps are spread throughout the notebook so you can rerun each section independently, but make sure to run the loading of data before any other cell, otherwise the notebook breaks.
