# Predicting Readmission in Patients with Diabetes Mellitus
## Contributors
- Vivian Do
- Bethany Wang 

## Problem Statement
Rehospitalizations impose a significant financial burden on the healthcare system. According to the Center for Health Information and Analysis, hospital readmissions cost Medicare $26 billion annually, with $17 billion considered avoidable (Reardon, 2015). These avoidable readmissions contribute to the rising healthcare costs and strain resources for both patients and healthcare providers. The Hospital Readmission Reduction Program (HRRP), established by the Centers for Medicare and Medicaid Services (CMS), aims to address this issue. Under the program, hospitals are evaluated based on their ability to manage excess readmission and can face payment deductions as a consequence for poor performance (CMS.gov, 2023). 
   
This data science project serves to contribute to the ongoing efforts to reduce hospital readmissions. We focus specifically on diabetes mellitus encounters and hope to gain valuable insights into the risk factors associated with readmission in diabetic patients. This targeted approach serves as a stepping stone towards a broader goal of predicting readmissions for other chronic diseases. Accurately predicting hospital readmission for diabetic patients has two major benefits. First, healthcare providers can identify patients who are most at risk and intervene in a timely manner. Secondly, there are financial incentives for reducing admissions for hospitals in an effort to keep costs down and prevent financial penalties. These advantages emphasize the importance of developing an accurate predictive model for diabetes with the potential for wider application in other chronic diseases. 

## Data Source
   The original data comes from the Health Facts database and represents 10 years (1999-2008) of clinical patient records at 130 hospitals and integrated delivery systems  across the United States. The dataset used for this project contains a subset of this database as extracted by Strack et al. in their journal article [“Impact of HbA1c Measurement on Hospital Readmission Rates: Analysis of 70,000 Clinical Database Patient Records”](https://www.hindawi.com/journals/bmri/2014/781670/) (2013). The extracted dataset, accessed through the UCI Machine Learning Repository, contains 101766 patient encounters and 50 features that satisfy the following criteria:
   
- It is an inpatient encounter (a hospital admission)
- It is a “diabetic” encounter (i.e “diabetes” was entered into the system as either a primary/secondary diagnosis) 
- The length of stay was between 1-14 days
- Laboratory tests were performed during the encounter
- Medications were administered during the encounter (Strack et al., 2013). 
      
The 50 features can be divided into three subcategories: (1) patient demographics including race, gender, weight, payer code, (2) admission information including discharge type, admission source, admission type, whether the patient was readmitted, and (3) laboratory and medical interventions during the encounter including number of medications administered and procedures performed, blood glucose test (A1c) result, and the change in dosage for a number of drugs ([UCI Machine Learning Repository, 2014](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)). 
