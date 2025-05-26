## Analysis of Results By Scenario
This file contains the analysis of the results obtained after the evaluation step by scenario.

## Experimental Setup and Results

Experiments were conducted to evaluate the system's performance on the following task:

- [Task 1: ensure exhaustive coverage of the system's defined technical scenarios]
- [Task 2: demonstrate the cross-domain generalizability of our approach through its application to heterogeneous datasets]
- [Task 3: empirically assess the pertinence of the generated reduction suggestions, both in terms of alignment with technical compatibility and preservation of task-specific performance]

### 1. Healthcare \& Medical Diagnostics 

Dataset: [Heart Attack Prediction](https://www.kaggle.com/datasets/juledz/heart-attack-prediction)

Priority Order: Reduced size → Interpretability → Performance → Computational cost
- In medical contexts, datasets often involve high-dimensional patient data. Reduced size is prioritized to improve model robustness and mitigate overfitting.
- Interpretability is crucial because clinicians must understand and trust model decisions, especially in high-stakes scenarios.
- While performance is important, it’s acceptable to slightly compromise accuracy for transparency.
- Computational cost is less critical due to access to hospital infrastructure or cloud computing.

#### Obtained Results

![Heart Attack Prediction](.github/assests/images/1.Medical.png)

#### Technical Compatibility with the Reduction Techniques

![Technical Compatibility with the Reduction Techniques](.github/assests/images/1.RedTech.png)

#### Priority Compatibility

1. Reduced size - Retained Options:
![](.github/assests/images/1.RedTech.png)   
3. Interpretability - Retained Options:

5. Performance - Retained Options:

7. Computational cost - Not Necessary:

---

### 2. Tourism \& Hospitality Management 

Dataset: [Hotel Booking](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)

Priority Order: Computational cost → Performance → Reduced size → Interpretability
- In hospitality systems (e.g., booking platforms), fast and cost-efficient decisions are essential for handling large volumes of user requests in real-time.
- Performance matters for ensuring booking accuracy and user satisfaction.
- Reduced size is secondary, useful for reducing latency.
- Interpretability is less crucial as decisions affect revenue but not human health or safety.

#### Obtained Results

![Hotel Booking Prediction](.github/assests/images/2.Hotel.png)

#### Technical Compatibility with the Reduction Techniques

![Technical Compatibility with the Reduction Techniques](.github/assests/images/2.RedTech.png)

#### Priority Compatibility

1. Reduced size - Retained Options:
   
3. Interpretability - Retained Options:

5. Performance - Retained Options:

7. Computational cost - Not Necessary:

---

### 3. Sociodemographic Studies \& Public Policy 

Dataset: [Housing](https://www.kaggle.com/datasets/camnugent/california-housing-prices)

Priority Order: Performance → Computational cost → Reduced size → Interpretability 
- In policy-making, accurate prediction or classification of social phenomena is central for resource allocation and planning.
- Computational cost is considered because these studies often use large government datasets.
- Reduced size is valued to ensure feasibility on standard infrastructure.
- Interpretability is less critical as decisions are aggregated and not made at the individual level.

#### Obtained Results

![Housing](.github/assests/images/3.Housing.png)

#### Technical Compatibility with the Reduction Techniques

![Technical Compatibility with the Reduction Techniques](.github/assests/images/3.RedTech.png)

#### Priority Compatibility

1. Reduced size - Retained Options:
   
3. Interpretability - Retained Options:

5. Performance - Retained Options:

7. Computational cost - Not Necessary:

---

### 4. Finance \& Risk Management 

[Company Bankruptcy Prediction](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction)

Priority Order: Performance → Computational cost → Reduced size → Interpretability 
- Financial systems require high-performing models for forecasting, fraud detection, and risk assessment.
- Computational efficiency is vital due to the volume and velocity of financial data.
- Reduced size improves real-time applicability.
- While interpretability is helpful (e.g., for regulatory compliance), it often takes a back seat to predictive accuracy in trading and risk scenarios.

#### Obtained Results

![Company Bankruptcy Prediction](.github/assests/images/4.Bankruptcy.png)

#### Technical Compatibility with the Reduction Techniques

![Technical Compatibility with the Reduction Techniques](.github/assests/images/4.RedTech.png)

#### Priority Compatibility

1. Reduced size - Retained Options:
   
3. Interpretability - Retained Options:

5. Performance - Retained Options:

7. Computational cost - Not Necessary:

---

### 5. Agriculture \& Food Safety 

[Mushrooms Classification](https://www.kaggle.com/datasets/uciml/mushroom-classification)

Priority Order: Computational cost → Performance → Reduced size → Interpretability 
- In field-based applications, computational efficiency is a priority due to the use of edge devices (e.g., sensors, drones).
- Performance is key for real-time classification (e.g., plant health, mushroom edibility).
- Reduced size supports deployment on lightweight systems.
- Interpretability is useful but not mission-critical for automated decisions.

#### Obtained Results

![Mushrooms Classification](.github/assests/images/5.Mushrooms.png)

#### Technical Compatibility with the Reduction Techniques

![Technical Compatibility with the Reduction Techniques](.github/assests/images/5.RedTech.png)

#### Priority Compatibility

1. Reduced size - Retained Options:
   
3. Interpretability - Retained Options:

5. Performance - Retained Options:

7. Computational cost - Not Necessary:

---

### 6. Urban Planning \& Real Estate Economics 

[Boston House Pricing](https://www.kaggle.com/datasets/fedesoriano/the-boston-houseprice-data)

Priority Order: Performance → Interpretability → Reduced size → Computational cost 
- Here, performance is necessary to provide reliable estimates for housing policies or economic forecasts.
- Interpretability is important to justify decisions to public officials or stakeholders.
- Reduced size supports usability across different municipalities.
- Computational cost is typically not a limiting factor, as analysis can be done offline.

#### Obtained Results

![Boston House Pricing](.github/assests/images/6.Boston.png)

#### Technical Compatibility with the Reduction Techniques

![Technical Compatibility with the Reduction Techniques](.github/assests/images/6.RedTech.png)

#### Priority Compatibility

1. Reduced size - Retained Options:
   
3. Interpretability - Retained Options:

5. Performance - Retained Options:

7. Computational cost - Not Necessary:

---

### 7. Education \& Academic Analytics 

[Students Performance](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)

Priority Order: Reduced size → Performance → Interpretability → Computational cost 
- In academic research, smaller datasets are easier to collect, share, and analyze across institutions.
- Performance ensures valid predictions of student outcomes.
- Interpretability helps explain model decisions to educators or policymakers.
- Computational cost is generally low-priority in academic settings, where time and resources are more flexible.

#### Obtained Results

![Students Performance](.github/assests/images/7.Students.png)

#### Technical Compatibility with the Reduction Techniques

![Technical Compatibility with the Reduction Techniques](.github/assests/images/7.RedTech.png)

#### Priority Compatibility

1. Reduced size - Retained Options:
   
3. Interpretability - Retained Options:

5. Performance - Retained Options:

7. Computational cost - Not Necessary:

---

### Evaluation Metrics 

- Performance based scoring function
  ° input: Accuracy, Precision, Recall, F1-score, and ROC AUC
  ° output: General score to asses whether a dataset remains suitable for classification
- Extent of data reduction
