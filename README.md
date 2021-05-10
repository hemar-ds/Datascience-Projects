#Survival analysis post bone marrow transplant based on Cognitive abilitities

##Project overview
Originally, clinicians were disinclined to recommend allogeneic HCT to elderly patients due to post-transplant survival issues. However, with the emergence of better supportive care and conditioning treatments, it has become a potentially viable option for patients of all ages. Determining how suitable an elderly patient would be for allogeneic HCT based on certain risk factors would help to inform clinicians about which patients would likely survive transplantation as part of their cancer treatment. 
There are studies and clinical trials being carried out in very recent years to include geriatric assessment scores to determine patients’ post-transplant survival rates. 
One emerging and quite exciting assessment that has potential as an indicator is the BOMC test which assesses cognitive ability. The question we want to answer is the following: ‘Will using cognitive ability alone as a predictor for survival in elderly patients with leukaemia perform as well as a well-known risk factor such as age?’.
There is an assumption that cognitive ability declines with age and therefore we believe it should perform similarly but cognitive ability is a fairly new risk factor that isn’t considered as much as age in actual clinics. The results of this analysis could provide evidence on how this should change and how cognitive ability should be more widely considered. 
Answering this question using machine learning may help give more support to this area of cancer treatment that is now beginning to be researched.

##Dataset:
The dataset we will be using has been taken from the following web page:
https://www.cibmtr.org/ReferenceCenter/PubList/PubDsDownload/Pages/default.aspx
It can be downloaded in the row for publication ‘Geriatric assessment in older alloHCT recipients: Association of functional and cognitive impairment with outcomes.’ by Rebecca Olin. 

##Evidence of permission to use the dataset:
The pdf can be downloaded by clicking on ‘View the Terms and Conditions.’ just above the table accessed through the above link (same as dataset link). 

##Technologies:
This project is created with Python V3

##Project status:
Complete, in EDA; during dataset exploration, we found out that most people have the leukemia-type disease; therefore, we looked at leukemia patients to allow a more fair comparison between patients. Handling missing Values, we used IterativeImputer to replace the missing values, which will reduce the risk of bias in the results. After this, we selected the features based on correlation and visualized the distribution. In feature scaling, splited the data into train test functions, and as the features were not normally distributed, we used standardization to bring the values in the same range. After this, we wanted to see if there is an association between certain features assessed in real-life clinics for elderly patients undergoing transplant and their non-relapse mortality/survival. We created different bar charts and boxplots to see any patterns between the features and survival and look at the distribution of data. Following this, we worked on Survival Analysis and Feature Selection, in which we used Kaplan-Meier Survival plots. After this, we started working on Model Building; we created different models, KNN Classifier, Decision Tree Classification, XGBoost, Random Forrest, SVM, Multi-Layer Perceptron (MLP), and created a Consolidated Metrics for Clinical Features and Geriatric Features. From these comparisons, we can see that the KNN model is the best model for both the clinical features and the geriatric features models. Statistically compared these two models to see if there is a significant difference in their performances 


