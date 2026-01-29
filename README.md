# 🎭 LLM Persona-Bias Analysis

### Automated Framework for Testing LLM Robustness Against Social Engineering

![Status](https://img.shields.io/badge/Status-Research_Phase-blue) ![Language](https://img.shields.io/badge/Language-Python_3.10-green) ![Focus](https://img.shields.io/badge/Focus-AI_Security-red)

## 📌 Project Overview
**LLM Persona-Bias Analysis** is a research project dedicated to investigating the vulnerability of Large Language Models (LLMs) to **Persona-based Attacks**. 
Unlike traditional adversarial attacks that use gibberish or complex algorithms, this project focuses on **Social Engineering**: forcing the model to adopt specific roles (e.g., "The Developer," "The Grandmother," "The Victim") to bypass Safety Guardrails.

The goal is to statistically measure how different "Personas" affect the **Attack Success Rate (ASR)** on restricted topics.

## 🎯 Objectives
1.  **Library Creation:** Build a dataset of 20+ System Prompts representing various social roles.
2.  **Automated Testing:** Develop a pipeline to test 100+ unsafe queries (from AdvBench) against these personas.
3.  **Analysis:** Generate a "Vulnerability Heatmap" showing which roles are most dangerous for AI safety.

## 🛠 Methodology
The research follows a Black-Box approach:
1.  **Input:** Malicious query (e.g., "How to bypass firewall").
2.  **Wrapper:** The query is wrapped into a specific Persona Context.
3.  **Inference:** Request sent to target models (GPT-4o, Llama-3, etc.).
4.  **Evaluation:** Automatic classification of the response (Refusal vs. Jailbreak).

## 📂 Project Structure
* `src/` - Source code for the attack pipeline.
* `data/` - Datasets (Personas, AdvBench subset).
* `notebooks/` - Jupyter notebooks for data analysis and visualization.
* `results/` - Logs and Heatmaps.

## 🚀 Roadmap
- [x] **Checkpoint 1 (Jan 30):** Topic approval, architecture design, repository setup.
- [ ] **Checkpoint 2 (Feb 03):** Baseline script implementation, first successful manual jailbreaks.
- [ ] **Checkpoint 3 (Final):** Full automated pipeline, comparative analysis, final report.

## 👤 Author
* **Sergey** - *Lead Researcher*
