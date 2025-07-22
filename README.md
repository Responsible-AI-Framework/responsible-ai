
This contains source for the paper title "**Regulation of AI Models: A Systematic and Responsible Approach**"

## Abstract

Artificial intelligence systems increasingly influence decisions in high-stakes domains such as healthcare, finance, and public services. In these settings, responsible AI refers to developing and deploying models that not only perform accurately but also meet essential standards of transparency, fairness, and environmental efficiency. However, current evaluation practices often treat these dimensions separately, making it difficult to compare models holistically or align them with ethical and regulatory expectations. This paper addresses that gap by introducing a unified evaluation framework that systematically quantifies model responsibility across three core dimensions: explainability, fairness, and computational sustainability. Using 18 established metrics, the framework generates normalized scores for each dimension along with an aggregated Responsibility Score to support transparent, reproducible, and context-sensitive comparisons. We apply the framework to three representative model architectures: a multi-layer perceptron, a deep residual network, and a tree-based ensemble, using public tabular datasets from financial, healthcare, and socioeconomic domains. All models are trained to comparable accuracy levels to ensure fair comparison. Results reveal consistent trade-offs: tree-based models provide stronger explainability and energy efficiency, while deep networks perform better on fairness but consume more resources. By translating ethical considerations into measurable indicators, the framework offers a practical tool for developers, auditors, and regulators. It supports informed model selection, prioritization based on domain needs, and alignment with emerging standards for responsible AI deployment.

## Pipeline

This proposed framework is applied to three commonly used model architectures on public tabular datasets across key real-world domains: finance, healthcare, and socioeconomics:

- **Credit**: A financial dataset used for classifying credit default risk.
- **Diabetes**: A healthcare dataset aimed at predicting the onset of diabetes using diagnostic features.
- **Income**: A socioeconomic dataset designed to predict whether an individual's income surpasses $50K per year based on census information.

The framework evaluates popular model architectures along three core dimensions of AI responsibility:

- **Explainability**: The ability to clarify how an AI model links inputs to outputs in a way that reveals its reasoning.
- **Fairness**: The model’s capacity to make decisions that do not systematically favor or disadvantage any group represented in the data.
- **Sustainability**: The computational and environmental costs associated with training, deploying, and maintaining machine learning models.

Evaluated models:

- **XGB** (eXtreme Gradient Boosting): A tree-based ensemble method.
- **MLP** (Multi-Layer Perceptron): A variance of feedforward neural network.
- **TabResNet**: A deep residual network adapted for tabular data.

<p align="center">
  <img src="figures/pipeline.png" alt="Pipeline" width="90%">
</p>

The evaluation of each dataset across all models for all dimension scores alongside their final responsibility score and accuracy is illustrated as follows:

<p align="center">
  <img src="figures/results.png" alt="Results" width="90%">
</p>



## Installation

1. Clone the repository:

```bash
git clone https://github.com/responsive-ai-framework/responsive-ai.git

``` 

2. Install dependencies:

```bash
cd responsive-ai
pip install -r requirements.txt
```

## Usage

To run the experiments, you need to run each notebook individually, and the results is achieved at the end of each session.