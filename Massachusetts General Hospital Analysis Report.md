Massachusetts Hospital Analysis

📚 Table of Contents
1 📌 Introduction
2 📝 Project Description
3 🎯 Project Aim
4 🛠️ Tools and Technology 
5 📁 About the Dataset
6 📋 Dataset Overview
7 📥 Importing the Dataset
8 🧹 Data Cleaning & Transformation
9 📐 Data Modeling
10 📈 Data Analysis
11 📊 Data Visualization
12 🔍 Key Insights
13 ✅ Recommendations
14 📌 Conclusion

📌 Introduction:
The Massachusetts General Hospital dataset project is a data-driven initiative that explores synthetic patient records from MGH between 2011 and 2022. Developed as part of a public data science effort, the dataset includes 974 patient profiles, capturing a wide range of healthcare metrics. This enables analysis of trends in patient care, such as readmission rates, procedure frequency, and insurance distribution. Also assesses hospital efficiency using metrics like length of stay and visit frequency. Highlighting disparities in race, ethnicity, and insurance coverage among patients.

📝 Project Description:
This project offers a comprehensive data-driven evaluation of Massachusetts General Hospital (MGH), designed to uncover the hidden dynamics behind patient care, hospital operations, and financial performance. It combines clinical data (patients demographics and procedure records), insurance records, and encounter histories to answer critical questions about how hospitals functions.
Key Components of the Analysis:
•	Patient Demographics: Age, gender, and other attributes that influence care delivery and resource allocation.
•	Hospital Encounters: Trends in inpatient, outpatient, and emergency visits across time.
•	Procedure Volumes & Costs: Identification of high-frequency and high-cost medical procedures.
•	Insurance & Payers: Breakdown of coverage types and their impact on hospital revenue.
•	Performance Metrics: KPIs related to efficiency, cost management, and clinical outcomes.
The DAX power query used to extract and analyze key metrics such as readmission rates, length of stay average length of stay.
Visualization was done with Power BI dashboards created to present findings in an interactive and accessible format.

🎯 Project Aim:
The Massachusetts General Hospital dataset project is aimed at evaluating hospital performance and patient care trends with key business questions below to be addressed.
•	What percentage of patients are readmitted within 30 days?
•	Are patients with specific insurance types paying more out-of-pocket?
•	Do patients with public insurance or no insurance tend to have longer stays or delayed treatments?
•	Which patient demographics (age, gender, race and ethnicity) are linked to longer hospital stays?
•	What is the average length of stay (LOS) across all patients?
•	Do older patients have higher readmission rates or longer stays?
•	Which demographic groups are most likely to experience complications or incur higher costs?

🛠️ Tools and Technology:
Excel and Power BI: For data cleaning, transformation, modeling, visualization, and storytelling.

📁 About the Dataset:
This dataset is a representation of patient records from Massachusetts General Hospital.  This is an imitation of a real-world hospital operations while upholding privacy and ethical standards.

📋 Dataset Overview:
•	Source: Skills to Career Mentorship
•	Timeframe: 2011–2022
•	Size: 974 patient profiles
•	Structure: Composed of 5 relational tables:
•	Patients: Demographics including age, gender, race, and ethnicity
•	Encounters: Records of inpatient, outpatient, and emergency visits
•	Procedures: Medical procedures performed during encounters
•	Payers: Insurance coverage details
•	Organizations: Facility or department information
The entire dataset comprised of 76,647 rows and 55 columns.
Patients Table:
•	Patient ID: Unique identifier for each patient
•	Birthdate: Used to calculate age
•	Gender, Race, Ethnicity, Demographic attributes
Encounters Table:
•	Encounter ID: Unique visit identifier
•	Patient ID: Foreign key linking to the patient
•	Encounter Type: Inpatient, outpatient, emergency
•	Start Date, End Date: Used to calculate length of stay
Procedures Table:
•	Procedure ID: Unique procedure identifier
•	Encounter ID: Links to the related medical visit
•	Code, Description: Type of procedure performed
•	Cost: Estimated cost of the procedure
Payers Table:
•	Payer ID: Insurance provider identifier
•	Name: Insurance company name
•	Coverage Type: Public, private, or uninsured

📥 Importing the Dataset:
The data file was received as a CSV files then it was merged the files into one Excel file but different sheets. Tables were created for each of the sheets, then save it as MGH Dataset.
The files were formatted before been imported to Power BI. The importing process involves going to power BI and using the ‘Get Data’ function to import the entire dataset into Power BI. 
I had to establish a relationship between all the tables by using the primary key. This is done by using the modelling function to with the help of the primary keys to establish relationship between the tables. 

🧹 Data Cleaning & Transformation:
Steps taken to clean and prepare the data:
•	Removed duplicates became possible with the use of the power query editor.
•	Fixed missing values with the replacement of the ‘null’ values with ‘0’, ‘blank’ or empty values with unknown.
•	Standardized column names by deleting unnecessary columns and making the necessary columns into uniform fonts.
•	Changed data types from text to numbers for date and time, from text to currency for encounter cost, etc. 

📐 Data Modeling:
16 DAX measures and 7 columns were created using the DAX function in Power BI.

📈 Data Analysis:
•	Admission Date, Discharge Date and readmission rate
•	Average Length of Stay
•	Patients Demographics (Age, Gender, Race and Ethnicity)
•	Encounter Cost, Total Claim Cost 
•	Insurance Coverage. 

📊 Data Visualization:
Dashboard/Page 1: Patients Overview
•	KPI Cards: Total Patients, Male, Female and Marital Status Slicer
•	Pie Chart: Length of Stay by Gender and Marital Status
•	Bar Chart: Length of Stay by Race and Readmission Rate by Race.
Dashboard/Page 2: Demographics
•	Ribbon Chart: Age Groups Distribution
•	Bar Chart: Ethnicity
•	Line Chart: Year and Ethnicity.
•	Funnel Chart: Descriptions 
Dashboard/Page 3: Readmission Trends & KPIs
•	KPIs: Average Length of Stay, Total Admission, Total Readmission, and Percentage Readmission within 30 Days
•	Bar Chart: Distribution by encounter class and Age Group
•	Line Chart: Readmission Rates by Months.
Dashboard/Page 4: Insurance coverage 
•	KPIs: Total Insurance coverage, Total base encounter cost, Total Claim cost, and Total Payment by patients.
•	Bar Charts: Patients payment distribution, Out of pocket Payment by Patient.
•	Tables: Average Length of Stay Distribution and Out of Pocket Distribution.

🔍 Key Insights:
•	There is 17.63% of readmission within 30 days and this may suggest a potential gap in discharge planning, follow up care or the effectiveness of the treatment previously received.
•	This indicates that patients with No-insurance tends to pay more out of pocket which means this may not fully cover procedures, medications or diagnostics.
•	The highest number of Length of Stay picked in 2014 with 706 and 3179 for Hispanics and non-Hispanics and 2021 with 716 and 2814 for Hispanics and non-Hispanics respectively while the elderly of Age Group 91-100 had the highest count of length of stay.
•	Older patients may have to stay longer due to their slower recovery rates and higher prevalence of some chronic ailments; for the gender, the female tends to stay longer due to post-surgical recovery, or maternity related issues but the males may stay longer as a result of trauma or cardiovascular diagnosis.
•	4.81 is the average Length of Stay and knowing the length of stay either nationally or regionally will help to tailor this insight properly.

✅ Recommendations:
•	There should be a Standardized Discharge Protocol in place that will ensure every patient receives clear, written discharge instructions, including medication schedules, warning signs, and follow-up appointments.
•	When possible, recommend lower-cost procedures without compromising care quality. Also explain billing expectations and available support during discharge or consultation.
•	Implement specialized care protocols for the oldest patients, focusing on early mobility, nutrition, and cognitive support to reduce LOS. Also, equip staff to understand cultural preferences and barriers that may affect recovery and discharge readiness.

📌 Conclusion:
•	High 30-Day Readmission Rate (17.63%)
Indicates possible gaps in discharge planning, follow-up care, or treatment effectiveness.
•	Uninsured Patients Face Higher Out-of-Pocket Costs
Suggests limited access to procedures, diagnostics, and medications, potentially leading to delayed or incomplete care.
•	Length of Stay (LOS) Peaks in 2014 & 2021
Non-Hispanics had higher LOS counts than Hispanics; elderly patients aged 91–100 had the longest stays.
Potential Impact on Business Decisions: 
•	Reducing readmissions can lower costs and improve patient outcomes, boosting hospital performance metrics.
•	Streamlining discharge planning and follow-up care can reduce LOS and improve bed turnover efficiency.
•	Addressing uninsured patient burdens can improve billing recovery rates and reduce bad debt.
•	Consider bundled payments or sliding scales to make care more accessible and predictable.
•	Develop culturally competent care models for Hispanic populations and tailored medical services for the elderly.
•	Use LOS and readmission trends to allocate staff, beds, and post-acute care resources more effectively.





