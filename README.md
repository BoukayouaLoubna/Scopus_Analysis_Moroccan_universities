# 📊 Moroccan Universities Scopus Analysis

### **Prepared By** 
- Boukayoua Loubna 
- Bachiri Jawad   
- El Boutaheri Najma  

**Supervised By:** Mr. Anass El Haddadi  
**Institution:** Abdelmalek Essaadi University  
**School:** National School of Applied Sciences, Al Hoceima  


## 🔎 **Introduction**
The project aims to analyze scientific publications from Moroccan universities using data sourced from **Scopus**. The objective is to:

- Evaluate academic performance.
- Identify research trends and international collaborations.
- Highlight dominant research fields.
- ... 

This analysis provides **strategic insights** to strengthen the impact of Moroccan academic institutions.


## 🚀 **Project Description**
The project is centered on:  
1. Collecting and preprocessing **Scopus** data.  
2. Building a data model and visualizations to analyze academic outputs.  
3. Generating meaningful insights into collaborations, publications, and research themes.



## 🛠️ **Project Architecture**
The architecture showcases the end-to-end workflow for the "Moroccan Universities Scopus Analysis" project.  
It includes data ingestion, transformation, storage, modeling and visualization stages

![ProjectArchitecture](https://github.com/user-attachments/assets/2bfb2f25-19cb-43df-ae82-33a5a0a046a5)

### Architecture Overview
Data is extracted from Scopus via an API.
Raw data is stored securely in Snowflake.
Transformation processes (cleaning, preprocessing, and modeling) are applied using PySpark.
Fact and dimension tables are stored in SQL Server.
Dashboards are built using Power BI to visualize trends, insights, and key metrics.

### **Tools & Technologies Used:**
- **Scopus and its Api**: Data soursce
- **Snowflake**: Raw Data storage.
- **pyspark**: Data Preprocessinh and analysis
- **SQL Server**: data model
- **Power BI**: Data visualization.  


## 📂 **Dataset**

**Data Source:**
- The raw data originates from Scopus, an academic research database.
- Data is fetched via an API to extract relevant information about publications, authors, collaborations, and more.

- **Tables**: 6 main tables  

**Data Categories Include:**  
1. Author Information  
2. Publication Details  
3. Citations and References  
4. Affiliations and Conferences  
5. Geographical Insights  


## 🔧 **Data Preprocessing**

The following extraction and preprocessing steps were performed:

1. **Data Extraction**:  
   - Authors Table  
   - Affiliations Table  
   - Geographic Table (Countries, Cities)  
   - Moroccan and Foreign Universities  

2. **Data Transformation**:  
   - Extracted author IDs and split names using **regular expressions**.  
   - Integrated affiliations and publication metadata.



## 📊 **Data Modeling**

### **Dimension Tables**:

| Table Name      | Attributes                                |
|-----------------|-------------------------------------------|
| `Dim_Author`    | id_author, full_name_author, email        |
| `Dim_Affiliation` | id_affiliation, university_name         |
| `Dim_Geographic` | id_geo, city, country                   |
| `Dim_Publication` | id_publication, title, abstract, language |
| `Dim_Web`       | id_web, DOI, link, relation              |
| `Dim_Conference` | id_conference, name, start_date, end_date|

### **Fact Table**:

| Table Name      | Attributes                                |
|-----------------|-------------------------------------------|
| `Fact_Global`   | id_author, id_affiliation, id_geo, id_publication, id_conference, id_web, year, global_index |



![image](https://github.com/user-attachments/assets/cc8944f5-765c-40d2-8c80-83e6c13b3d16)



## 📈 **Key Visualizations**

![image](https://github.com/user-attachments/assets/08eee270-56c5-4bcc-80a2-2280056d03bb)


![Screenshot 2024-12-26 121237](https://github.com/user-attachments/assets/84463fd5-2d48-48a2-9972-30efd8604d17)


![Screenshot 2024-12-26 121305](https://github.com/user-attachments/assets/d327b629-7806-4964-b328-80b6d2822a06)

### check the link below for project insights

[View Dashboards](https://app.powerbi.com/view?r=eyJrIjoiMTQwYTFmOTktZTQwMS00ZjQxLWFmNmEtMzNhNGQ2ZDA4YTkxIiwidCI6ImMyNzg3OTIyLTExZDktNGNhOC1hYWRmLTVlZjdmZjMxYTEyNyJ9)


1. **Geographical Distribution of Publications**:  
   - Analysis of Moroccan vs. International universities.  

2. **Collaboration Analysis**:  
   - Researcher and institutional collaboration networks.  

3. **Temporal Trends**:  
   - Study of publication trends over time.  

4. **Thematic Analysis**:  
   - Dominant research themes extracted from publication titles and abstracts.  

5. **Social Network Mining**:  
   - Visualizing research collaboration networks.


## 📌 **Insights**

- **58%** of publications originate from Moroccan universities.  
- **42%** represent collaborations with foreign institutions.  
- Major trends include **geographical, temporal, and thematic analysis** of Moroccan research outputs.  


## 🎯 **Conclusion**

This project highlights:  
- The strong academic contributions of Moroccan universities.  
- Collaboration trends and thematic focuses to guide future strategies.  
- The importance of data-driven insights for decision-making in academia.



## 👥 **Team Contributions**

This project was a result of collaborative efforts.  
All team members worked together on data collection, preprocessing, analysis, modeling and visualization to ensure the success of this project.  
Each member actively contributed to every stage, showcasing strong teamwork and shared responsibility. 


## 📧 **Contact**

For inquiries, please contact:  
- loubnaboukayoua@gmail.com
