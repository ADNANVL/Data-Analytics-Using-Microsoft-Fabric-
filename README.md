# News-Analysis-Using-Microsoft-Fabric

🚀 Azure Data Engineering project: News Analysis 📈


In this project, I have created an end to end solution for analyzing the latest news data. I have used the microsoft fabric for all the tools. Here's a 
breakdown of the journey:


![workflow](https://github.com/ADNANVL/Data-Analytics-Using-Microsoft-Fabric-/blob/main/Microsoft%20Fabric%20Tools.png)

1️⃣ Data Ingestion: Created pipeline in data Factory which connects to Bing API and ingest all the latest news articles as a raw json structure to the lakehouse.
Source Code = https://github.com/ADNANVL/Data-Analytics-Using-Microsoft-Fabric-/tree/main/Data%20Ingestion

2️⃣ Synapse Data Engineering: Used synapse data engineering component to read the ingested raw json file and process it to a clean and structured Delta table and load that into the same Lakehouse database.
Spark Code = https://github.com/ADNANVL/Data-Analytics-Using-Microsoft-Fabric-/blob/main/Data%20Transformation/process_news_data.ipynb

3️⃣ Synapse Data Science: used this to read this clean Delta table and sentiment analysis is performed further by using a description column which contains information 
about the news articles so basically we use this information and predicted the sentiment of the news using a pre-trained synapse machine learning model and the data 
is stored as a Delta table in the Lakehouse.
Spark Code = https://github.com/ADNANVL/Data-Analytics-Using-Microsoft-Fabric-/blob/main/Sentiment%20Analysis/News_Sentimental_Analysis.ipynb

4️⃣ PowerBI Dashboard - Created two page report one page was autocreated by powerbi and then I created a new page which is our main news dashboard based on 
requirements in this dashboard I have configuration in a way that every time when I open this report only the latest news that are published in the last 24 hours will 
be displayed.
Dashboard = https://github.com/ADNANVL/Data-Analytics-Using-Microsoft-Fabric-/tree/main/PowerBI%20Report

![Screenshot (270)](https://github.com/ADNANVL/Data-Analytics-Using-Microsoft-Fabric-/blob/main/Final%20Pipeline/Pipeline.png)
![Screenshot 2024-04-23 145306](https://github.com/ADNANVL/Data-Analytics-Using-Microsoft-Fabric-/blob/main/PowerBI%20Report/News_Dashboard_.pdf)

