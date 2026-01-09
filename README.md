# 🧠 Psychographic Cyber Targeting
*A Computational Framework for Psychographic Profiling in Digital Environments*
[![Open In Colab](https://colab.research.google.com/github/RosariaCDiLauro/psychographic-profiling-experiment/blob/main/psychographic-profiling-experiment.ipynb)


**Author:** Rosaria Chiara Di Lauro

---

## 📑 Table of Contents
1. [Project Overview](#project-overview)  
2. [Scientific Context](#scientific-context)  
3. [Research Objective](#research-objective)  
4. [Dataset and Data Source](#dataset-and-data-source)  
5. [System Architecture](#system-architecture)  
6. [Psychographic Dimensions](#psychographic-dimensions)  
7. [Vulnerability Modeling](#vulnerability-modeling)  
8. [Contextual (Subreddit) Analysis](#contextual-subreddit-analysis)  
9. [Output and Interpretation](#output-and-interpretation)  
10. [Reproducibility and Scientific Use](#reproducibility-and-scientific-use)  
11. [Ethical and Methodological Note](#ethical-and-methodological-note)  
12. [License](#license)

---

## Project Overview

This repository contains a **computational framework for psychographic profiling** designed to analyze how emotional patterns, personality traits, and discursive environments interact to produce **cognitive and emotional vulnerability** in digital users.

The system processes large-scale social media data (Reddit posts and comments) and extracts:

- Emotional distributions  
- Big-Five personality traits (OCEAN model)  
- Dominant discussion environments  
- Group-level vulnerability patterns  

The final goal is to model how **psychological profiling can support cyber targeting and influence operations**, as explored in the associated master’s thesis:

> **“Psychographic Profiling: The Role of Psychology in the Cyber Targeting Process”**

---

## Scientific Context

Modern cyber operations increasingly rely on **psychological targeting** rather than purely technical exploits.  
Influence campaigns, disinformation, and psychological operations (PSYOPs) operate by identifying **who is cognitively and emotionally vulnerable** to specific types of persuasion.

This project integrates three scientific domains:

- **Computational social science**  
- **Personality psychology (OCEAN / Big Five)**  
- **Emotion analysis (multi-label affective classification)**  

into a single pipeline that allows **data-driven psychographic profiling at scale**.

---

## Research Objective

The core objective is to answer the following research question:

> *Can computational models combining emotions, personality traits, and discursive context identify differential vulnerability to targeted psychological influence in online environments?*

Rather than focusing on individual users, the system operates on **clusters and groups**, identifying **psychographic profiles** that are more or less susceptible to persuasion, emotional manipulation, and narrative framing.

---

## Dataset and Data Source

The framework operates on Reddit data structured in tabular format.  
Each row represents a user-generated contribution with the following information:

- Author  
- Subreddit (context)  
- Text content  
- Predicted emotions (multi-label)  
- Predicted personality traits (OCEAN scores)

The emotional labels are based on a fine-grained affective taxonomy (anger, fear, sadness, joy, disgust, etc.), while personality traits follow the **Big Five model**:

- Openness  
- Conscientiousness  
- Extraversion  
- Agreeableness  
- Neuroticism  

---

## System Architecture

The pipeline implemented in the notebook follows these stages:

1. **Data loading and preprocessing**  
2. **Emotion normalization and aggregation**  
3. **Personality trait aggregation at user and group level**  
4. **Subreddit (context) extraction**  
5. **Psychographic cluster computation**  
6. **Vulnerability scoring**  
7. **Interpretation and reporting**

Each step transforms raw textual signals into **structured psychological indicators** that can be used to reason about targeting potential.

---

## Psychographic Dimensions

Two primary dimensions are extracted:

### Emotional Structure
The model computes:
- Dominant emotions  
- Emotional volatility  
- Conflict-oriented vs regulation-oriented affective patterns  

### Personality Structure
Based on OCEAN:
- Neuroticism and Openness are treated as vulnerability amplifiers  
- Conscientiousness and emotional regulation as stabilizers  

These dimensions are combined to build **psychographic fingerprints** of groups.

---

## Vulnerability Modeling

Vulnerability is not defined as a single variable but as a **multidimensional construct** emerging from:

- High emotional reactivity  
- Negative or conflict-oriented emotional clusters  
- Personality configurations associated with anxiety, openness to influence, or cognitive instability  

The framework computes a **vulnerability score** for each group by integrating these components.

This score is designed to represent **susceptibility to targeted persuasion and narrative manipulation**.

---

## Contextual (Subreddit) Analysis

The system extracts the dominant subreddits associated with each group, allowing the identification of:

- Generalist vs niche communities  
- Political, social, or identity-based spaces  
- Emotional climates of different discursive environments  

Importantly, the system shows that **vulnerability is not determined by the platform itself**, but by the interaction between:

> personality × emotion × context

---

## Output and Interpretation

The notebook produces:

- Group-level emotional profiles  
- Personality trait distributions  
- Dominant discussion environments  
- Vulnerability indices  
- Interpretative summaries  

These outputs allow researchers to reason about **which types of audiences are more likely to be influenced by cyber-psychological operations**.

---

## Reproducibility and Scientific Use

This project is designed as a **reproducible experimental framework**.

The notebook:
- Can be rerun on any compatible dataset  
- Produces transparent intermediate outputs  
- Supports comparative group analysis  

This makes it suitable for:
- Academic replication  
- Methodological validation  
- Extension to other platforms or datasets  

---

## Ethical and Methodological Note

The dataset used does **not** originate from real military or intelligence operations.  
It represents **open, civilian online discourse**.

Therefore:
- The framework demonstrates **methodological feasibility**
- Not operational deployment  

The goal is to show how such techniques **could be used**, not that they are already being applied in these datasets.

---

## License

This project is released under the **MIT License**, allowing free use, modification, and academic or industrial application with proper attribution.  
See the [LICENSE](LICENSE) file for full terms and conditions.
