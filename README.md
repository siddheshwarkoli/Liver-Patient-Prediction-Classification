# Liver-Patient-Prediction-Classification

# LIVER PATIENT

## <b>PROBLEM CONTEXT
##### <b>Patients with Liver disease have been continuously increasing because of excessive consumption of alcohol, inhale of harmful gases, intake of contaminated food, pickles and drugs.

##### <b>This dataset was used to evaluate prediction algorithms in an effort to reduce burden on doctors.

## <b>CONTENT
<b>This data set contains 416 liver patient records and 167 non liver patient records collected from North East of Andhra Pradesh, India.<br>
<b>The "Dataset" column is a class label used to divide groups into liver patient (liver disease) or not (no disease).<br>
<b>This data set contains 441 male patient records and 142 female patient records.<br>
<b>Any patient whose age exceeded 89 is listed as being of age "90".<br>

## <b>FEATURES:
<b>
    
- Age of the patient
- Gender of the patient
- Total Bilirubin
- Direct Bilirubin
- Alkaline Phosphotase
- Alamine Aminotransferase
- Aspartate Aminotransferase
- Total Protiens
- Albumin
- Albumin and Globulin Ratio
- Dataset: field used to split the data into two sets (patient with liver disease, or no disease)

### <b>TYPES OF MACHINE LEARNING PROBLEM.
- <b>It is a binary classification problem, where given the above set of features, we need to predict if a given patient has liver disease or not.<br>
### <b>LIST OF ALGORITHMS USES FOR CLASSIFICATION
<b>
    
- Logistic Regression
- Support Vector Classification (SVC)
- K-Nearest Neighbors (KNN)
- Decision Tree Classifier
- Random Forest
- Gradient Boosting Machines (GBM)
- XGBoost
- Naive Bayes


## <b>DOMAIN ANALYSIS


- <b>Total Bilirubin</b><br>
This is a blood test that measures the amount of a substance called bilirubin.<br>
A small amount of bilirubin in your blood is normal, but a high level may be a sign of liver disease.<br>

- <b>Direct Bilirubin</b><br>
Bilirubin is a substance made when your body breaks down old red blood cells<br>
A small amount of bilirubin in your blood is normal. Healthy adults make 250 to 350 milligrams (mg) of bilirubin each day.<br>

- <b>Alkaline Phosphotase</b><br>
An alkaline phosphatase (ALP) test measures the amount of ALP in your blood.<br>
ALP is an enzyme found throughout the body, but it is mostly found in the liver, bones, kidneys, and digestive system.<br>
When the liver is damaged, ALP may leak into the bloodstream. High levels of ALP can indicate liver disease or bone disorders.<br>
An alkaline phosphatase test is used to detect diseases of the liver or bones.<br>

- <b>Alamine Aminotransferase</b><br>
An enzyme found in the liver and other tissues.<br>
A high level of Alkaline Aminotransferase released into the blood may be a sign of liver damage, cancer, or other diseases.<br>
Also called alanine transferase and serum glutamate pyruvate transaminase.<br>

- <b>Aspartate Aminotransferase</b><br>
An enzyme found in the liver, heart, and other tissues.<br>
A high level of Aspartate Aminotransferase released into the blood may be a sign of liver or heart damage, cancer, or other diseases.<br>
Also called aspartate transaminase and serum glutamic-oxaloacetic transaminase.<br>

- <b>Total Proteins</b><br>
The total protein test measures the total amount albumin and globulin in your body.<br>
It’s used as part of your routine health checkup.<br>
It may also be used if you have unexpected weight loss, fatigue, or the symptoms of a kidney or liver disease.<br>

- <b>Albumin</b><br>
Albumin is a protein made by the liver.<br>
A serum albumin test measures the amount of this protein in the clear liquid portion of the blood.<br>
Albumin can also be measured in the urine.<br>
Blood is drawn from a vein (venipuncture), usually from the inside of the elbow or the back of the hand.<br>

- <b>Albumin_and_Globulin_Ratio</b><br>
A total protein and albumin/globulin ratio test measures the total amount of protein in your blood

# <b>TASK 1
#### <b>PREPARE A COMPLETE DATA ANALYSIS REPORT ON THE GIVEN DATA.

# <b>TASK 2
#### <b>CREATE A PREDICTIVE MODEL WITH IMPLEMENTATION OF DIFFERENT CLASSIFIERS ON LIVER PATIENT DISEASES DATASET TO PREDICT LIVER DISEASES.

# <b>TASK 3
#### <b>CREATE AN ANALYSIS TO SHOW ON WHAT BASIS YOU HAVE DESIGNED  YOUR MODEL.

# <b>SUMMARY OF PROJECT

#### <b> This analysis explains the rationale behind the choices made during the design of the liver disease prediction model.

#### <b> 1. Dataset Understanding
- The dataset includes **numerical** and **categorical** features.
- The target variable is binary: **1 = Liver Patient**, **2 = Not a Liver Patient**.
- Some features contain **missing values** (e.g., 'Albumin_and_Globulin_Ratio').

#### <b> 2. Data Preprocessing
- **Missing Value Imputation**:
  - Numerical: Median imputation (robust to outliers).
  - Categorical: Most frequent imputation (to preserve mode).
- **Feature Scaling**:
  - Applied `StandardScaler` to normalize numerical features.
- **Categorical Encoding**:
  - `Gender` column encoded using `OneHotEncoder` to make it numerical.

#### <b> 3. Model Selection
Multiple models were tested to find the best performing classifier:

| Model               | Reason for Inclusion                                  |
|---------------------|--------------------------------------------------------|
| Logistic Regression | Simple, interpretable, good baseline.                 |
| Decision Tree       | Captures non-linear patterns, interpretable.          |
| Random Forest       | Robust ensemble method, handles variance well.        |
| SVM                 | Effective for higher-dimensional separation.          |

#### <b>4. Train-Test Split
- Used an **80/20 split** to evaluate model generalization.
- Ensures that the test set is representative but not too small.

#### <b> 5. Evaluation Metrics
- Used `classification_report` to evaluate:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1-score**
- These metrics provide a detailed performance overview, especially useful for imbalanced datasets.

#### <b> 6. Model Interpretation
- Random Forest was initially preferred due to its balance between performance and interpretability.
- If needed, feature importance can be extracted to understand contributing variables.

# <b>END OF PROJECT
<b>SIDDHESHWAR KOLI
