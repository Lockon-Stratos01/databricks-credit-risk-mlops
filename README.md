# databricks-credit-risk-mlops
Pipeline de Machine Learning para avaliação de risco de crédito com Databricks, MLflow e Random Forest.

# 🏦 Machine Learning no Databricks: Predição de Risco de Crédito com MLflow

[![Databricks](https://img.shields.io/badge/Databricks-Serverless-FF3621?logo=databricks&logoColor=white)](#)
[![MLflow](https://img.shields.io/badge/MLflow-Tracking-0194E2?logo=mlflow&logoColor=white)](#)
[![Python](https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white)](#)
[![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-ML-F7931E?logo=scikitlearn&logoColor=white)](#)

## 📌 Visão Geral do Projeto
Este projeto desenvolve um pipeline de Machine Learning de ponta a ponta para avaliação de concessão e risco de crédito em clientes bancários. Todo o desenvolvimento, treinamento e rastreamento de experimentos foi realizado na plataforma **Databricks**, utilizando **MLflow** para governança do ciclo de vida dos modelos.

---

## 🛠️ Arquitetura e Tecnologias
- **Plataforma:** Databricks (Runtime Serverless)
- **Modelos:** Logistic Regression (Baseline) vs. Random Forest Classifier
- **Experiment Tracking:** MLflow (métricas, hiperparâmetros e artefatos)
- **Linguagem:** Python (Pandas, Scikit-Learn, NumPy)

---

## 📊 Comparação de Modelos (MLflow Tracking)

| Modelo | Accuracy | F1-Score | Status |
|---|---|---|---|
| Logistic Regression (Baseline) | 0.7450 | 0.2857 | Descartado |
| **Random Forest (Tuned)** | **0.7800** | **0.4210** | **Campeão (Em Produção)** |

> Evidência visual dos experimentos executados e registrados via MLflow:
> 
> *(Adicione o print do seu experimento aqui)*  
> `![Experimentos no MLflow](docs/mlflow_experiment.png)`

---

## 📂 Estrutura do Repositório
```text
├── notebooks/
│   └── 01_predicao_credito_mlflow.ipynb   # Notebook completo com treino e MLflow
├── docs/
│   └── mlflow_experiment.png              # Evidência visual dos experimentos
├── README.md                              # Documentação do projeto
└── LICENSE                                # Licença MIT
