# Probing Preverbs: Evaluating Large Language Models on Latin and Ancient Greek Preverbed Motion Verbs

This repository contains the data and code to reproduce the results from the paper, "Probing Preverbs: Evaluating Large Language Models on Latin and Ancient Greek Preverbed Motion Verbs."

Our study investigates the ability of 13 Large Language Models (LLMs) to interpret the semantics of preverbs in Latin and Ancient Greek. Preverbs—prefixes that modify verbal bases—present a complex challenge for computational models due to their semantic spectrum, ranging from fully compositional to highly lexicalized and idiomatic meanings.

## Abstract

> Preverbs, i.e., prefixes that modify verbal bases, play a central role in the semantics of Latin and Ancient Greek. Their meanings range from fully compositional to highly lexicalized, making them an ideal test case for evaluating the semantic capacities of Large Language Models (LLMs). We investigate the ability of 13 LLMs to interpret preverb semantics across a dataset of 2,834 manually annotated preverbed motion verbs, under zero-, one-, two-, and five-shot prompting conditions. We find that LLMs perform moderately well overall, with GPT-5 achieving the highest F1 of 0.629. Performance improves with increased context examples and is generally higher for compositional, non-lexicalized preverbs, Ancient Greek, and earlier historical periods. Qualitative evaluation highlights systematic differences in consistency, sensitivity to lexicalization, and handling of polysemy, revealing that reasoning-enabled and larger models tend to generate more accurate and internally coherent interpretations. These results provide insight into the capacities and limitations of current LLMs for modeling morpheme-level semantics in historical languages, with implications for philology, digital humanities, and the development of linguistically informed AI systems.

## Repository Structure

This repository is organized as follows:

-   **`preverb_semantics_evaluation.ipynb`**: A Jupyter Notebook containing the Python code used to analyze the model predictions. It allows for the replication of our quantitative evaluation.
-   **`results/`**: This directory contains the raw predictions from all 13 Large Language Models evaluated in our study.
    -   The `results` directory is organized into subfolders, one for each model family (e.g., `gpt-5`, `qwen`, `deepseek`, `llama`).
    -   Inside each subfolder, you will find CSV files corresponding to different prompting conditions (zero-shot, one-shot, two-shot, and five-shot).

### Data Format

The CSV files follow a consistent naming convention: `results_<model_name>_<shot_condition>.csv`. For example: `results_deepseek-reasoner_five_shot.csv`.

Each file contains the model's predictions, including the target verb, the context sentence, the gold-standard annotation(s), and the model's predicted preverb meaning(s).


## Citation

If you use the data or code from this repository in your research, please cite our paper:

[To be updated after publication]
