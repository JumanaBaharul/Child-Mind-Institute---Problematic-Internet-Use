# Problematic Internet Use Prediction Model
This project leverages the Healthy Brain Network (HBN) dataset to predict the Severity Impairment Index (SII), a measure of problematic internet use in children and adolescents. Using accessible physical fitness and activity data as proxies, we aim to identify early indicators of unhealthy internet habits, promoting healthier digital behavior.

## Challenge Description
Problematic internet use among children and adolescents is a growing concern in today's digital age. Existing methods to measure this issue often require professional assessments, leading to access, cultural, and linguistic barriers. This project proposes utilizing easily obtainable physical fitness indicators as proxies to detect problematic internet use, particularly in contexts lacking clinical expertise.

## Dataset
**Demographics:** Age and sex data.< br / >
**Internet Use:** Daily usage hours.< br / >
**Physical Measures:** Metrics like blood pressure, heart rate, BMI, and fitness assessments.< br / >
**Questionnaires:** Sleep disturbances, physical activity levels, and internet addiction.< br / >
**Target Variable**: PCIAT_Total-derived SII (Severity Impairment Index) with four levels: None, Mild, Moderate, and Severe.< br / >
Approach
We implemented multiple predictive models, combining dimensionality reduction techniques and boosting algorithms, to analyze physical activity data and predict SII levels. The core architecture used was a Sparse Autoencoder (SAE), paired with ensemble learning models such as LightGBM, XGBoost, and CatBoost. Key variations included:

**Enhanced Normalization:** Layer normalization for training stability.< br / >
**Advanced Activation:** Leaky ReLU for improved gradient flow.< br / >
**Dropout Regularization:** To prevent overfitting.< br / >
**Sparse Representations:** Efficient feature encoding.< br / >

## Results and Conclusion
Among the various model architectures, the Sparse Autoencoder (SAE) + XGBoost achieved the best performance:< br / >

Mean Train QWK: 0.9255< br / >
Mean Validation QWK: 0.4996< br / >
Optimized QWK SCORE: 0.538< br / >
The Sparse Autoencoder successfully captured high-dimensional patterns, while XGBoost effectively handled non-linear relationships in the data. This combination proved to be robust and efficient, setting a benchmark for predicting problematic internet use based on physical activity data.

# Future Scope
**Integration with Wearable Technology:** Real-time monitoring for immediate feedback and intervention.< br / >
**Personalized Interventions:** Tailored strategies for reducing internet use based on individual data.< br / >
**Cross-Disciplinary Collaboration:** Involving experts in psychology, education, and technology for a holistic approach.< br / >
**Natural Language Processing (NLP):** Analyzing social media and online communication for early signs of problematic behavior.< br / >
