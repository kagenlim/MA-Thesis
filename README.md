# MA-Thesis

My M.A. Thesis is titled 'Quantifying Variation in American School Safety with Explainable Machine Learning: An Application of Machine Learning Feature Importances for the Social Sciences'. On this repository, I share the code that I have used to generate the results in my thesis. This includes Python and R code, as well as some LaTeX code that was used to generate regression and summary statistics. The results from the Python and R scripts have been knit into HTML files, for your ease of viewing. Please do reach out if there is any way that I can help!


> Abstract: 
Social scientists, methodologists and policy analysts often work with datasets that contain numerous potential explanatory variables, which contain a mix of data types (e.g., survey items measured on different scales). This presents unique challenges for considering these variables within the same model. An approach utilizing machine learning feature importances, a key metric of explainable machine learning, is illustrated through an investigation of variation in American school safety along markers of student disadvantage (e.g., students with low grades, or students who do not regard academic achievement as important). This study is based on the 2017–2018 School Survey of Crime and Safety (SSOCS) conducted by the United States Department of Education, which captures perceptions and responses from school leaders, on the safety conditions of their respective schools. After an illustrative example based on a conventional linear regression approach, random forest regressors are fit and tuned on a theoretically-relevant subset of features in this dataset. SHapley Additive exPlanation (SHAP) values were then calculated from the tuned random forest regressor model, as feature importance metrics for each feature and observation in the data. Results indicate that schools with a higher percentage of disadvantaged students and/or schools that implemented random sweeps were, on average, less safe. On the other hand, schools that implemented parental involvement strategies were, on average, more safe. The value of this explainable machine learning approach for the school safety literature, policy analysis and wider social and behavioural research is also discussed, along with limitations and future directions on how SHAP values could be employed for social science research.

>Keywords: Explainable Machine Learning, Linear Regression, Random Forests, SHapley Additive exPlanations, American School Safety

Guide to this Repository: 

- `pu_ssocs18.sav`: The public access 2017–2018 School Survey of Crime and Safety (SSOCS) dataset used in this thesis. This was obtained from the website of the National Center for Education Statistics (https://nces.ed.gov/pubsearch/pubsinfo.asp?pubid=2020054). To make sense of this, please go onto NCES' website to download the full dataset and other relevant materials as a zip file, as well as the comprehensive codebook by Zoe Padgett and colleagues to make sense of the variables. Please do note that NCES has a Data Usage Agreement, which legally prohibits any attempt to determine the identity of any reported case. This dataset may only be used for statistical purposes. 
- `preprocessed_data.csv`: This is the processed data that has been preprocessed through `Preprocessing_Script.Rmd`.
- `Preprocessing_Script.Rmd`, `Regressions_Script.Rmd`, `ML_Script.ipynb`: R and Python code for the data preprocessing, feature engineering, analyses and visualizations used in my thesis. 
- `KagenLim_MAThesis_ExplainableMachineLearningSchoolSafety.pdf`: This is my M.A. thesis manuscript. 

- `HTML_Output_Scripts`: HTML output from the R and Python scripts.
- `LaTeX_Code_Tables`: LaTeX code used to generate regression and summary statistics tables. 
- `SHAP_Values`: DataFrames of SHAP Values for the Explainable Machine Learning component of my thesis, as well as descriptive statistics tables as csv files. 
- `Slide_Deck`: I had the opportunity to talk about this work at an event. These are my slides.
