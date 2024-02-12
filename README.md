# Tokyo Olympics Data Analysis Pipeline on Azure

<p>This project implements an end-to-end data pipeline built on Microsoft Azure technologies to analyze data related to the Tokyo Olympics.
Utilizing a combination of Azure Data Factory, Databricks, Data Lake Storage, and Synapse Analytics, the pipeline ingests, transforms, stores, and analyzes data sourced from Kaggle.</p>

<h2>Data Source</h2>
The dataset used in this project is obtained from Kaggle (<a href="https://www.kaggle.com/datasets/arjunprasadsarkhel/2021-olympics-in-tokyo?resource=download">Kaggle Dataset</a>).
<p>This contains the details of over 11,000 athletes, with 47 disciplines, along with 743 Teams taking part in the 2021(2020) Tokyo Olympics.
The dataset contains the details of the Athletes, Coaches, and Teams participating as well as the Entries by gender. It contains their names, countries represented, disciplines, gender of competitors, and names of the coaches.</p>

<h2>Pipeline Architecture</h2>

[![Project-Architecture.jpg](https://i.postimg.cc/XvH3wFMV/Project-Architecture.jpg)](https://postimg.cc/zLg9NyXM)
<ul>
<li><strong>Data Source:</strong> The pipeline starts by accessing the dataset from the local storage.</li>
<li><strong>Azure Data Factory:</strong> This service acts as the orchestration engine, automating data movement and transformations throughout the pipeline.</li>
<li><strong>Data Lake Storage:</strong> Raw data retrieved from Kaggle is initially stored in the Data Lake for temporary staging.</li>
<li><strong>Azure Databricks:</strong> This Spark-based analytics platform performs data cleaning, transformations, and feature engineering on the raw data.</li>
<li><strong>Data Lake Storage:</strong> Transformed data is stored back in the Data Lake for further analysis.</li>
<li><strong>Azure Synapse Analytics:</strong> This cloud-based data warehouse stores the final, transformed data and enables complex SQL queries for analysis.</li>
</ul>

[![Resources-Used-Azure.png](https://i.postimg.cc/43Ns7PSL/Resources-Used-Azure.png)](https://postimg.cc/Jsg9SNmZ)

<br>

<h2>Analysis</h2>
The pipeline enables analysis of the Tokyo Olympics data using complex SQL queries within Synapse Analytics.
Examples of analysis questions include:
1. Identifying top-performing countries and athletes across different disciplines.
2. Most Bronze, silver, and gold-winning nations.
3. Coaches vs Player Ratio.
4. Sports with Highest female participation.

<h2>Benefits</h2>
<ul>
<li>This pipeline offers a scalable and efficient solution for analyzing large datasets like the Tokyo Olympics data.</li>
<li>Azure services provide a managed environment, simplifying infrastructure management and maintenance.</li>
<li>The modular architecture allows for easy updates and additions to the data processing and analysis steps.</li>
<li>The pipeline facilitates data exploration and discovery through interactive SQL queries in Synapse Analytics.</li>
</ul>
