# Responsible AI

This repository contains the source code and experimental framework for the paper:

**_Regulation of AI Models: A Systematic and Responsible Approach_**

---

## 🔍 Overview

Artificial intelligence is increasingly used in high-stakes domains like healthcare, finance, and public services. However, current evaluation methods rarely assess AI models holistically. This project introduces a unified framework for evaluating **model responsibility** across:

- **Explainability**: How transparently the model links input to output  
- **Fairness**: How equitably it treats different demographic groups  
- **Sustainability**: How efficiently it consumes computational resources

Using **18 established metrics**, the framework produces:
- Normalized scores per dimension
- A final **Responsibility Score** for each model

---

## ⚙️ Method

We apply the framework to three widely used model types:
- **XGBoost**: Tree-based ensemble
- **MLP**: Multi-layer perceptron
- **TabResNet**: Residual neural network for tabular data

All models are trained to comparable accuracy and evaluated on three public tabular datasets:
- `Credit` – Financial risk prediction
- `Diabetes` – Medical diagnosis prediction
- `Income` – Socioeconomic income classification

<p align="center">
  <img src="figures/pipeline.png" alt="Pipeline" width="90%">
</p>

---

## 📊 Results

Our framework enables responsible model selection by exposing clear trade-offs:
- **Tree-based models**: High explainability and low carbon cost
- **Deep networks**: Better fairness, higher computational burden

<p align="center">
  <img src="figures/results.png" alt="Results" width="90%">
</p>

---

## 📦 Installation

```bash
git clone https://github.com/responsible-ai-framework/responsible-ai.git
cd responsible-ai
pip install -r requirements.txt
