---

# MedBot – AI Powered Healthcare Chatbot for Disease Prediction

## Project Overview

MedBot is an AI-powered healthcare chatbot designed to assist users in identifying possible diseases based on their symptoms. The system uses Natural Language Processing (NLP), fuzzy logic, and ensemble machine learning models to analyze user-provided symptoms and predict potential diseases.

Users interact with the chatbot by entering symptoms in natural language. The system extracts relevant medical terms, processes them using fuzzy matching to handle variations in wording, and predicts the most likely disease using multiple machine learning models.

The final prediction is generated using an ensemble majority voting approach, improving reliability and accuracy across different disease classes.

---

# Introduction

Many people search online for health-related symptoms before consulting a doctor. However, symptom descriptions may vary due to **different word choices, spelling variations, or synonyms**.

MedBot addresses this challenge by combining **NLP techniques with fuzzy systems** to correctly interpret similar symptoms such as:

* "stomach pain"
* "abdominal pain"
* "belly ache"

By recognizing similar meanings and mapping them to standardized symptoms, the system improves prediction accuracy.

The chatbot supports disease prediction for multiple health conditions, helping users gain preliminary insights before seeking professional medical advice.

---

# Diseases Supported

The system predicts the following diseases:

* Diabetes
* Asthma
* Gastroenteritis
* Pneumonia
* Osteoarthritis

Each disease is predicted based on a combination of symptoms provided by the user.

---

# Key Features

• AI-based healthcare chatbot interface
• Natural Language Processing for symptom extraction
• Fuzzy logic for handling similar or misspelled symptom words
• Ensemble learning for improved prediction accuracy
• Multi-disease classification
• Interactive conversation-based symptom input

---

# System Architecture

The system consists of several key components:

1. User Input (Symptom description)
2. NLP Symptom Extraction
3. Fuzzy Matching System
4. Feature Vector Generation
5. Ensemble Machine Learning Models
6. Majority Voting Prediction
7. Chatbot Response

---

# Natural Language Processing (NLP)

The chatbot processes user input using NLP techniques to extract symptoms from free text.

Example input:

```
I have been feeling chest tightness and difficulty breathing
```

Extracted symptoms:

* chest tightness
* breathing difficulty

The extracted symptoms are converted into a structured format for machine learning models.

---

# Fuzzy Logic for Symptom Matching

Different users may describe the same symptom using different words.

For example:

| User Input      | Standard Symptom    |
| --------------- | ------------------- |
| belly pain      | abdominal pain      |
| stomach ache    | abdominal pain      |
| breathing issue | shortness of breath |

A **fuzzy matching system** is implemented to map similar or misspelled words to standardized symptoms.

This improves the system’s ability to understand real-world user inputs.

---

# Machine Learning Models

The system uses multiple machine learning models for disease prediction.

## 1. Naïve Bayes

A probabilistic classifier commonly used for text classification tasks. It calculates the probability of diseases based on observed symptoms.

## 2. Recurrent Neural Network (RNN)

RNN is used to capture sequential patterns in symptom descriptions and improve prediction accuracy for complex symptom combinations.

## 3. Support Vector Machine (SVM)

SVM is used for classification by finding optimal decision boundaries between disease classes.

---

# Ensemble Learning

Instead of relying on a single model, MedBot uses an **ensemble approach**.

### Majority Voting Method

1. Each model predicts a disease.
2. Predictions from all models are collected.
3. The disease predicted by the majority of models becomes the final prediction.

This approach improves:

* Accuracy
* Stability
* Prediction reliability

---

# Workflow

1. User enters symptoms in natural language.
2. NLP module extracts key symptoms.
3. Fuzzy system standardizes symptom names.
4. Symptoms are converted into a feature vector.
5. Multiple machine learning models predict diseases.
6. Majority voting determines the final prediction.
7. Chatbot returns the predicted disease to the user.

---

# Example Interaction

User Input:

```
I have fever, cough, and trouble breathing
```

System Processing:

* Extracted symptoms → fever, cough, breathing difficulty
* Fuzzy matching → standardized symptoms
* Model predictions → Pneumonia

Chatbot Response:

```
Based on the symptoms provided, the predicted condition is Pneumonia.
Please consult a healthcare professional for proper medical diagnosis.
```

---

# Technologies Used

• Python
• Natural Language Processing (NLP)
• Scikit-learn
• TensorFlow 
• Fuzzy Matching Algorithms
• Machine Learning Ensemble Methods

---


# Applications

• AI-powered healthcare chatbots
• Early disease screening systems
• Telemedicine platforms
• Medical decision support systems

---

# Future Improvements

• Add more diseases and symptoms
• Integrate medical knowledge graphs
• Deploy as a web or mobile application
• Improve NLP using transformer models like BERT

---

# Author

**Tharun Kumar**

---
