# Data Mining Project
Healthcare Data Analysis & Predictive Modeling

This repository presents a structured analysis of a large healthcare dataset, focusing on uncovering the patterns that influence medical costs, admission behaviors, and diagnostic outcomes. The work combines exploratory analysis with a simple classification model built in RapidMiner, aiming to translate raw data into practical insights that support decision-making in healthcare settings.

⸻

📊 Dataset Overview

The dataset includes 55,500 patient records, covering a wide range of demographic, clinical, and administrative details such as:
	•	Age and gender
	•	Blood type
	•	Medical condition
	•	Admission and discharge dates
	•	Insurance provider
	•	Billing amount
	•	Diagnostic test result (Normal, Abnormal, Inconclusive)

The data is well-structured, with balanced gender and blood type distributions, making it a suitable foundation for both descriptive and predictive analysis.

⸻

🛠 Tools & Workflow

The project was developed using:
	•	RapidMiner Studio for preprocessing, feature engineering, and model building
	•	Excel for initial inspection
	•	(Optional) Python for any additional analysis or future work

Preprocessing

The dataset required minimal cleaning, as it contained no missing values or duplicated entries. A new attribute, Stay Duration, was created by calculating the difference between admission and discharge dates. Numerical fields such as age and billing amount were normalized to improve the stability of the model.

Exploration

Visualizations were used to examine key relationships, including:
	•	How test results differ across age groups
	•	Gender-based differences in chronic conditions
	•	The link between admission type and diagnostic outcome
	•	Billing variations among insurance providers
	•	Medical conditions associated with longer hospital stays

Modeling Approach

A Decision Tree classifier was used to predict the Test Result.
The original dataset showed class imbalance, so stratified sampling was applied. A sample size of 700 produced the most reasonable balance and allowed the model to recognize all three classes.

Model Performance:
	•	Accuracy: 32.67%
	•	Precision (weighted): 15.56%
	•	Recall (weighted): 32.93%

The model is intentionally simple. The goal was not high accuracy, but understanding the factors the tree relies on when making predictions.

⸻

✨ Key Findings
	•	Chronic conditions such as hypertension and diabetes become significantly more common with age.
	•	Women show higher prevalence of arthritis and asthma; men show more hypertension and diabetes.
	•	Emergency admissions tend to produce more abnormal test results.
	•	Billing amounts differ noticeably across insurance providers.
	•	Certain medical conditions naturally lead to longer hospital stays.
	•	Medication use reflects clear, condition-specific treatment patterns.

These findings help paint a wider picture of how demographics, health status, and administrative elements collectively shape patient outcomes and hospital costs.

⸻

🚀 Running the RapidMiner Model
	1.	Download the .rmp process file.
	2.	Open RapidMiner Studio.
	3.	Import the dataset.
	4.	Load the provided process.
	5.	Verify attribute roles (label and features).
	6.	Run the workflow to reproduce the evaluation and visualizations.
