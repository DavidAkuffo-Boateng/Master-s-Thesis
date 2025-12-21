Project Overview

This repository contains code and materials related to my MSc dissertation at the University of Stirling. The project investigates how compact language models perform on empathetic dialogue generation tasks, with a particular focus on data preprocessing, model efficiency, and contextual relevance.

The study compares two pre trained transformer based models, GPT 2 Small and DistilGPT, using the Empathetic Dialogues dataset. While this dataset has become a common benchmark for evaluating emotional responses in language models, existing work provides limited documentation on effective preprocessing strategies. This project addresses that gap by developing and applying a tailored preprocessing pipeline and evaluating its impact on model performance.

Research Focus

The primary objectives of this work were to:

1. Design a reproducible preprocessing pipeline for the Empathetic Dialogues dataset

2. Evaluate the performance of compact language models under different contextual settings

3. Examine trade offs between model size, response diversity, and adherence to emotional context

4. Assess whether smaller models can offer practical advantages in resource constrained settings

Methodology

The preprocessed dataset was used to evaluate GPT 2 Small and DistilGPT in zero shot, one shot, and five shot prompting scenarios. Model performance was assessed using perplexity and lexical similarity measured via cosine similarity.

These evaluation settings allowed for a structured comparison of how additional context influences response generation and emotional expression across models of different sizes.

Key Findings

The results reveal a nuanced relationship between model size, contextual input, and performance in empathetic dialogue tasks. As the number of shots increased, lexical similarity generally decreased, suggesting a trade off between response diversity and strict adherence to target phrasing.

Both models showed limitations in maintaining precise emotional context. However, DistilGPT, despite having fewer parameters, demonstrated more consistent improvements in general emotional expression as contextual information increased. This challenges the assumption that larger models necessarily perform better in few shot learning scenarios.

Contributions

This work makes two primary contributions:

1. A fully preprocessed version of the Empathetic Dialogues dataset, intended to support future research and reproducibility

2. Empirical evidence that compact language models can exhibit competitive and sometimes more stable behaviour in empathetic dialogue tasks, particularly when computational resources are limited

The findings suggest that efficiency should be treated as a central consideration when designing conversational AI systems for real world applications such as mental health support and customer service.

Thesis

The full dissertation is available in this repository as a PDF and provides detailed discussion of the experimental design, results, and implications of the study.
