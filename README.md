# Netflix-PowerBI-Analytics
End-to-end Netflix analytics dashboard using Power BI — data cleaning, DAX modeling, and interactive visual insights.
Objective

To build an interactive Power BI dashboard for exploring Netflix content insights by performing data cleaning, modeling, and visualization.

🛠 Tools Used

Power BI

Power Query (data cleaning)

DAX (KPI calculations)

📊 Key Features

Total Movies vs TV Shows

Year-wise content trend

Country-wise content distribution (Map)

Genre analysis

Search & filter capabilities (Genre, Country, Year)

🧹 Data Preparation

Removed duplicates

Cleaned null & inconsistent values

Converted date_added to date format

Extracted Year & Month

Standardized text fields

🧠 Main DAX Measures
Total Titles = COUNTROWS('netflix_titles')

Total Movies =
CALCULATE(COUNTROWS('netflix_titles'),
'netflix_titles'[type] = "Movie")

Total TV Shows =
CALCULATE(COUNTROWS('netflix_titles'),
'netflix_titles'[type] = "TV Show")
