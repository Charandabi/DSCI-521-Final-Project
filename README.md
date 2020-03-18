# DSCI-521-Final-Project

# SCREENING FOR CHRONIC KIDNEY DISEASE

Sina E. Charandabi, Thirukumaran Subramani, John Wilson
#### Drexel University

# Abstract
>_The purpose of this study is to create an efficient screening tool to identify patients at risk for chronic kidney disease (CKD). Despite the wide availability and low cost of a test for CKD based on one or more blood samples, studies have shown that many in the at-risk population have not been tested. One reason for this is that the awareness of CKD is low. Given the proven benefits of early detection and treatment, the need for some kind of screening tool is clear. Employing classification techniques, we will study how efficiently high-risk patients can be identified using easily obtainable patient data._


# Data

Since 1975, the National Center for Health Statistics of the Centers for Disease Control and Prevention has conducted nationwide surveys of U.S. adults. Using trained personnel, the center collected a wide variety of demographic and health information using direct interviews, examinations, and blood samples. The data set consists of selected information from 8,819 adults 20 years of age or older taken from the 1999 to 2000 and 2001 to 2002 surveys. The dataset is currently available at the following address from Darden Business Publishing: http://store.darden.virginia.edu/screening-for-chronic-kidney-diseaseDarden   

34 variables are included in the data set, where CDK, a 0/1 dummy variable, is the variable of interest,indicating whether or not a subject had CKD. Varibles, as defined in Table 1, are demographic in nature (variables 0 through 10), or were collected during the physical exam (variables 11 through 21), or aquired on self-reported health histories (variables 22 through 33). 

The first 50 observations from the dataset are represented in Table 2. Table 3 reports descriptive statistics for each of the numerical variables in dataset. 

# Outline of the Project

This project was developed in the following sections:

  - Phase 1: Project Scoping
   - Abstract
   - Introduction
   - Data and Variable Definition (Table 1)
   - Descriptive Statistics and Visualizations
   
  - Project Implementation
   - Data Preprocessing
    - Missing Values and Categorical Variables
    - Normalization
   - Making Predictions and Model Assessment
    -1. Unbalanced Data
      - 1.1. Inclusion of All Variables
      - 1.2. Excluding Highly-Correlated Variables
      - 1.3. Dimensionality Reduction Using Principle Components
      - 1.4. Keeping Variables Suggested by the Literature
    -2. Creating a Balanced Data
      - 2.1. Inclusion of All Variables
      - 2.2. Keeping Variables Suggested by the Literature
   - 3. Assesing the Logistic Regression Model
    - 3.1. Assessing the Performance by ROC Curve
    - 3.2. Discussion on the Statistical Significance
   - Concluding Remarks 

# Limitations

However, It is also important to note that because the study population is not a random sample of U.S. adults, any predictions suggested by current study requires further validation before utilizing for actual decision-making. 
