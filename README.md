# Sistema de Detecção de Fraude com MLflow

Este projeto implementa um sistema de Machine Learning end-to-end com foco em ML Systems, utilizando MLflow para rastreamento de experimentos, versionamento e monitoramento.

##  Objetivo

Detectar possíveis fraudes em transações utilizando um modelo pré-treinado da biblioteca Hugging Face.

---

##  Modelo Utilizado

- Modelo: facebook/bart-large-mnli  
- Tipo: Zero-shot classification  
- Biblioteca: Hugging Face Transformers  

---

##  Tecnologias

- Python  
- MLflow  
- Hugging Face Transformers  
- Scikit-learn  

---

##  Como Executar

### 1. Instalar dependências
pip install -r requirements.txt
### 2. Executar o pipeline
python src/train.py
### 3. Iniciar o MLflow
python -m mlflow ui
### 4. Executar inferência
python src/predict.py

---

##  Guardrails

O sistema implementa controle de confiança:

- Baixa confiança → recomendação de revisão manual  
- Alta confiança → alerta de possível fraude  

---

##  MLflow

O MLflow é utilizado para:

- Rastreamento de experimentos  
- Registro de métricas  
- Armazenamento de artefatos  
- Comparação de execuções  
