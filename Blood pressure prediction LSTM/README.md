# 🧠 Predicting Blood Pressure Spikes with LSTM + GenAI (RAG-powered Transparent AI)

## 📍 Author: Pradeep Gadanki

---

## 🔍 Overview

This project presents a hybrid AI solution that combines **LSTM Neural Networks** with **Generative AI** and **Retrieval-Augmented Generation (RAG)** to predict systolic and diastolic blood pressure levels in patients. The model not only forecasts BP trends from historical data but also integrates **explainable AI (XAI)** and **GenAI-backed clinical insights** to support medical decision-making.

Key innovations include:
- **Time-series LSTM modeling** of vital signs  
- **Explainability using SHAP, attention layers**  
- **RAG-enhanced justifications** with medical literature  
- **GenAI chatbot interface** for clinician and patient interaction

---

## 🧬 Motivation

Hypertension is a major contributor to cardiovascular disease and early detection of spikes can save lives. However, most AI models used in clinical prediction are black-boxes. This project solves that by offering:

- Accurate blood pressure forecasting using LSTM  
- Transparent model reasoning via SHAP and attention  
- RAG-based insights from clinical documents (AHA, WHO)  
- GenAI chatbot assistant for explainable interactions

---

## ⚙️ Tech Stack

| Category            | Tools & Frameworks                                  |
|---------------------|-----------------------------------------------------|
| **Language**        | Python                                              |
| **Modeling**        | TensorFlow, Keras (LSTM)                            |
| **Explainability**  | SHAP, Attention Layers, LIME                        |
| **GenAI**           | Hugging Face Transformers, GPT-4 / LLaMA2           |
| **RAG Pipeline**    | LangChain, FAISS / Weaviate                         |
| **Deployment**      | FastAPI, Docker                                     |
| **Visualization**   | Matplotlib, Seaborn                                 |
| **Data Handling**   | Pandas, NumPy                                       |
| **Evaluation**      | RMSE, MAE, R² Score                                 |

---

## 🩺 Dataset

- **Source**: Time-series health datasets (synthetic or anonymized real-world)
- **Features**:
  - Timestamps
  - Heart rate
  - Systolic & Diastolic BP
  - Age, weight, optional lifestyle/activity metrics
  - Metadata for retrieval (e.g., ICD codes, symptom tags)

---

## 💡 GenAI/RAG Features

- 🔍 **RAG Justification**: Fetches relevant clinical guidelines or research to explain each prediction  
- 🤖 **LLM-powered Insights**: Summarizes SHAP values in natural language using GPT-4  
- 💬 **Clinical QA Bot**: Interactive chatbot to answer queries on BP trends and model decisions  
- 🧭 **Explainability Dashboard**: Visual + narrative explanations for clinicians

---





### ⚙️ Install Dependencies

```bash
pip install -r requirements.txt


python src/genai/generate_explanations.py
uvicorn src.api.main:app --reload

