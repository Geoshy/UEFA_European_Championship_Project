# **UEFA European Championships Analysis Project**
![alt text](Figs/Project_Icon.png)

## **1. Introduction:**
This project analyzes the UEFA European Championships, providing insights into the trends, performances, and key moments that have defined one of the most prestigious football tournaments in the world. Using Python, data on the championships, spanning from 1960 to 2024, will be extracted from reliable sources such as official UEFA databases or Wikipedia. This data, encompassing match results, team performances, player statistics, and tournament outcomes, will then be loaded into Power BI Desktop. Within Power BI, the Extract, Transform, Load (ETL) process will be employed to clean, prepare, and structure the data, creating a robust foundation for analysis and reporting. The resulting visualizations will offer a comprehensive overview of the tournament's history, highlighting key performance indicators, team dominance, and emerging patterns within this dynamic and highly competitive football landscape.

You can see the full Dashboards from [here](Power_BI_Dashboards).

## **2. Tools I Used:**

**1. Python:** for extract the tables of the dataset from the Wikipedia website.

**2. Power BI Desktop:** for Extract, Transform, Load (ETL) process and create interactive dashboards.

**3. Git & GitHub:** for sharing my analysis and dashboard.

## **3. Extract Tables From Web _Wikipedia_ (UEFA European Championship):**
Using Python Pandas library to extract tables from the Wikipedia website from link: https://en.wikipedia.org/wiki/UEFA_European_Championship

```py
import pandas as pd

url = "https://en.wikipedia.org/wiki/UEFA_European_Championship"

tables = pd.read_html(url)

print(f"The Number Of Tables = {len(tables)}")

for index, table in enumerate(tables):
    print(f"Saving Table_{index + 1}")
    file_name = f"table_{index + 1}.csv"
    table.to_csv(
        file_name,
        index=False,
        header=True
    )
```
## **4. Upload Extracted Tables To Power BI Desktop:**

**4.1. Get data from Power BI using Text/CSV:**
![alt text](Figs/F2.PNG)

**4.2. Transform tables Into power query for cleaning and preparing structure the data:**

![alt text](Figs/F1.PNG)

## **5. Claening & Preparing The Data In Power Query:**

## **6. Create Measures For Analysis & Visualization:**

## **7. Dashboards:**

## **8. Analysis:**
