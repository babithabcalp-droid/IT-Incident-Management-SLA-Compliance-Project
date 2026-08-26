# IT Incident Management & SLA Compliance Dashboard
📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on an IT ticket dataset to understand incident management, Service Level Agreement (SLA) compliance, resolution times, and customer support performance.

The analysis uses Python to clean and preprocess the data, perform statistical analysis, explore relationships between different variables, and create visualizations to identify meaningful patterns and actionable insights.

The project follows a structured data analytics workflow:

Data Loading → Data Cleaning → Data Preprocessing → Exploratory Data Analysis → Statistical Analysis → Visualization → Insights & Recommendations

🎯 Objectives

The main objectives of this project are:

Understand the structure and quality of the IT ticket dataset.
Clean and preprocess the data for reliable analysis.
Analyze relationships between ticket priority, SLA compliance, and time variables.
Identify factors affecting SLA performance.
Analyze ticket resolution and first-response performance.
Explore customer survey results and agent interactions.
Create meaningful visualizations for better understanding.
Generate actionable insights and recommendations.
📊 Dataset

The dataset contains 1,515 IT support tickets and 20 features.

Main Features
Feature	Description
Status	Current status of the ticket
Ticket ID	Unique ticket identifier
Priority	Ticket priority level
Source	Channel through which the ticket was created
Topic	Type of issue reported
Agent Group	Team handling the ticket
Agent Name	Assigned support agent
Created time	Ticket creation timestamp
Expected SLA to resolve	Expected resolution SLA
Expected SLA to first response	Expected first-response SLA
First response time	Actual first response timestamp
SLA For first response	First-response SLA status
Resolution time	Ticket resolution timestamp
SLA For Resolution	Resolution SLA status
Close time	Ticket closure timestamp
Agent interactions	Number of agent interactions
Survey results	Customer feedback
Product group	Product/service category
Support Level	Support level such as L1, L2, or L3
Country	Country associated with the ticket

The notebook reports that the dataset contains no missing values across the analyzed columns.

🛠️ Technologies Used
Python
Pandas – Data manipulation and analysis
NumPy – Numerical operations
Matplotlib – Data visualization
Seaborn – Statistical visualization
Google Colab / Jupyter Notebook

🔍 Analysis Performed
1. Data Loading & Understanding
Imported the IT ticket dataset.
Examined the first and last records.
Checked dataset dimensions.
Reviewed column names and data types.
Inspected the overall structure of the dataset.
2. Data Preprocessing
Checked for missing values.
Examined duplicate records.
Converted and processed date/time fields.
Prepared variables for analysis.
3. Exploratory Data Analysis

The project explores:

Ticket status distribution
Ticket priority
Ticket sources
Ticket topics
Agent groups
Product groups
Support levels
Country-wise ticket distribution
Agent interactions
Customer survey results
SLA compliance
Resolution time
First response time
4. SLA Analysis

Both first-response SLA and resolution SLA are analyzed.

According to the notebook:

First-response SLA met: 96.2%
First-response SLA not met: 3.8%
Resolution SLA met: 98.5%
Resolution SLA not met: 1.5%

The analysis therefore shows stronger SLA performance for ticket resolution than for the initial response.

5. Statistical & Relationship Analysis

The project investigates relationships between:

First response time
Resolution time
Priority
Support level
Agent group
SLA compliance

Pivot tables are also used to summarize resolution SLA compliance by agent group and mean resolution time by priority and support level.

📈 Key Findings
SLA Performance

Overall SLA performance is strong, with resolution SLA compliance higher than first-response SLA compliance.

Response Time & Resolution Time

The analysis identifies a very strong correlation of 0.966 between first response time and resolution time. This indicates that improving the speed of the initial response should be an important operational priority.

Agent Groups

The analysis shows high resolution SLA compliance across agent groups. However, Customer Service and Development show slightly different SLA performance levels, making agent-group monitoring useful for operational improvement.

Priority

The project also examines resolution times across different priority levels and support levels to identify tickets that require additional attention.

💡 Recommendations

Based on the analysis:

Improve first-response time because it has a strong relationship with overall resolution time.
Closely monitor Customer Service and General Inquiry tickets because they show comparatively lower SLA performance.
Allocate resources according to country-wise ticket volume, particularly where demand is highest.
Monitor low-priority tickets, as they show substantially longer average resolution times.
Further analyze ticket complexity, agent workload, and escalation patterns to identify additional factors affecting SLA compliance.

📂 Project Structure
IT-Incident-Management-SLA/
│
├── Project_ITSM.ipynb
├── ITSM_Dataset.csv
├── README.md
└── images/
    └── visualizations/

Update the filenames above if your GitHub repository uses different file names.

▶️ How to Run the Project
1. Clone the repository
git clone https://github.com/your-username/IT-Incident-Management-SLA.git
2. Install required libraries
pip install pandas numpy matplotlib seaborn
3. Open the notebook

You can run the notebook using:

Jupyter Notebook
JupyterLab
Google Colab
4. Load the dataset

Place ITSM_Dataset.csv in the appropriate project directory and update the dataset path in the notebook if required.

📌 Conclusion

The analysis shows that the IT ticket-management process is performing well overall, with high SLA compliance across agent groups and topics.

The most important finding is the very strong relationship between first response time and resolution time. Therefore, improving the speed of the initial response can be an important strategy for improving overall ticket resolution performance.

The project demonstrates how Python-based data analysis and visualization can be used to evaluate IT service performance, identify SLA-related patterns, and support data-driven operational decisions.

👩‍💻 Author

Babitha Babu

Data Analytics Project

⭐ Skills Demonstrated
Data Cleaning
Data Preprocessing
Exploratory Data Analysis (EDA)
Statistical Analysis
Data Visualization
Correlation Analysis
Pivot Tables
SLA Analysis
Business Insights
Data-Driven Recommendations
