# Development and Internal Validation of Clinical Prediction Models for 7-Year Risk of MASLD

**A Prospective Population-Based Cohort Study in Iran (Amol Cohort Study)**

### Authors
Fahimeh Safarnezhad Tameshkel¹, Masoud Imani², Maziar Moradi-Lakeh³,*, Bahareh Amirkalali¹, Sahar Golpour-Hamedani¹, Azam Doost Mohammadian¹, Nima Motamed⁴, Mansoureh Maadi¹, Mehdi Nikkhah¹, Hadi Rezaei¹, Gholam Hossein Ashrafi⁵, Farhad Zamani¹*, Mohammad Hadi Karbalaie Niya¹,⁶

### Abstract
Metabolic dysfunction–associated steatotic liver disease (MASLD) affects approximately 38% of adults globally, making early identification of at-risk individuals critical for preventive intervention. This study developed and internally validated clinical prediction models for 7-year MASLD incidence using routinely available clinical parameters in an Iranian adult population. Data were drawn from the Amol Cohort Study, a prospective population-based cohort in northern Iran, enrolling adults aged ≥18 years between 2009 and 2010, with follow-up conducted between 2016 and 2017. Participants free of MASLD at baseline with complete follow-up outcome data were included; missing values in baseline predictor variables were addressed using multiple imputation by chained equations (MICE) rather than case exclusion. 

Sixteen demographic, anthropometric, laboratory, and clinical variables were used to train and compare five algorithms: logistic regression, random forest, XGBoost, naive Bayes, and multilayer perceptron. Models were evaluated using stratified 5-fold cross-validation within a 70% training set, followed by a single evaluation on an independent 30% hold-out test set. Incident MASLD was diagnosed via ultrasonography combined with cardiometabolic criteria. Of 2,588 eligible participants, 620 (24.0%) developed MASLD during follow-up. On the independent hold-out test set, random forest achieved the highest discrimination (ROC-AUC = 0.705), followed by XGBoost (0.699) and logistic regression (0.697). Logistic regression was retained as the primary predictive model given its direct clinical interpretability via odds ratios. BMI and alanine aminotransferase showed the largest effect sizes among the metabolic and laboratory predictors. These findings support logistic regression as a simple, interpretable approach for MASLD risk stratification.

### Repository Contents
* `MASLD_7Year_Prediction.ipynb`: The main Jupyter Notebook containing the full analysis pipeline, including data preprocessing, multiple imputation, model training, hyperparameter tuning, threshold optimization (Youden's J), bootstrap confidence intervals, calibration, and Decision Curve Analysis (DCA).
* `requirements.txt`: Python environment dependencies.

### Note on Data Privacy
Due to ethical restrictions and patient confidentiality guidelines (Ethics Committee of Iran University of Medical Sciences: IR.IUMS.FMD.REC.1403.312), the original patient-level dataset  cannot be shared publicly.

### How to Run
1. Clone this repository.
2. Install the dependencies: `pip install -r requirements.txt`
3. Run the Jupyter Notebook `MASLD_7Year_Prediction.ipynb`.
