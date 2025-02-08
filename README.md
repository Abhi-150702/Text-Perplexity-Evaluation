# Text-Perplexity-Evaluation-On-LLMs

### Benchmarking GPT-2 and GPT-Neo on Wikitext-2
This repository evaluates the performance of pre-trained language models such as GPT-2 (Standard & Medium) and GPT-Neo on the Wikitext-2 test dataset by computing perplexity. Additionally, it explores how minor text modifications such as typos or errors affect model performance.

### 🚀 Project Overview
The objective of this project is to analyze the robustness of GPT models when encountering modified text. By computing perplexity on both original and modified texts, we can assess how small changes impact model confidence.

### 📌 Steps to Complete the Task
- **Install Dependencies:** Ensure required libraries (```transformers```, ```datasets```, ```torch```, ```matplotlib```, ```seaborn```) are installed.
- **Load Pre-trained Models & Tokenizers:** Utilize Hugging Face’s ```transformers``` library to load GPT-2 and GPT-Neo.
- **Load Wikitext-2 Dataset:** Fetch the dataset using the ```datasets``` library.
- **Compute Perplexity:** Write a function to compute perplexity using the model's loss function.
- **Modify Text & Recompute Perplexity:** Introduce minor modifications (e.g., replacing ```"the"``` with ```"teh"```) and measure the impact.
- **Visualize Results:** Use histograms and line charts to compare perplexity distributions between original and modified texts.
- **Analyze Findings:** Compare mean perplexity scores for both cases.

### 📊 Visualizations
- **Histogram:** Shows the distribution of perplexity values for both ```GPT-2``` and ```GPT-Neo```.
- **Line Chart:** Compares the perplexity of original and modified texts across samples
- **Bar Chart:** Displays the mean perplexity values for each model.

### 📝 Results
- A higher perplexity score indicates lower model confidence in predicting the next word.
- Minor text modifications  impact perplexity, revealing model sensitivity to typos.
