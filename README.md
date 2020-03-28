# DSCI-521: Final-Project

# SCREENING FOR CHRONIC KIDNEY DISEASE

#### Drexel University, Department of Decision Science

# Abstract
>_The purpose of this study is to create an efficient screening tool to identify patients at risk for chronic kidney disease (CKD). Despite the wide availability and low cost of a test for CKD based on one or more blood samples, studies have shown that many in the at-risk population have not been tested. One reason for this is that the awareness of CKD is low. Given the proven benefits of early detection and treatment, the need for some kind of screening tool is clear. Employing classification techniques, we will study how efficiently high-risk patients can be identified using easily obtainable patient data._


# Data

The data set consists of selected information from 8,819 adults 20 years of age or older taken from the 1999 to 2000 and 2001 to 2002 surveys and is currently available at the following address from Darden Business Publishing: http://store.darden.virginia.edu/screening-for-chronic-kidney-diseaseDarden   

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
     - Unbalanced Data
        - Inclusion of All Variables
        - Excluding Highly-Correlated Variables
        - Dimensionality Reduction Using Principle Components
        - Keeping Variables Suggested by the Literature
     - Creating a Balanced Data
        - Inclusion of All Variables
        - Keeping Variables Suggested by the Literature
     - Assesing the Logistic Regression Model
        - Assessing the Performance by ROC Curve
        - Discussion on the Statistical Significance
    - Concluding Remarks 
    
# Required Libraries
- Pandas
- numpy
- seaborn
- matplotlib
- sklearn
- statsmodels

# Limitations

Because the study population is not a random sample of U.S. adults, any predictions suggested by current study requires further validation before utilizing for actual decision-making. 

After dropping observations containing missing values of CKD (the variable of interest), data becomes notably small which may be a challange for the performance of ML algorithms. To address this limitation, we imputed null values by the median of their associated variables. However, there are different features in the sklearn package to do this task better and can be utilized for next studies.

We were interested in reducing dimentionality using PCA method. However, as shown in the code file, fewer components fail to explain a large portion of variance in the model. Functionality of PCA in larger datasets can be further studied.

Another helpful area to explore this dataset is the implementation of unsupervised ML techniques such as neural networks and hierarchical clustering to find out potential commonalities between healthy objects or those affected by CKD.


