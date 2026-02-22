## Hi there, I'm Irinel 👋

Analytics Engineer with a passion for turning raw data into clear, actionable insights — whether that's through a well-structured pipeline, a polished Power BI report, or a chart that actually makes people stop and think.

I enjoy working across the full analytics stack: from wrangling data in Fabric pipelines and writing T-SQL queries, to crafting visuals in Power BI and exploring the boundaries of what BI tools can do. When I'm not doing that, I'm probably experimenting with something that has no direct business value but is a lot of fun to build.

---

## 🛠️ Tools & Technologies

**Data Engineering**

![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![T-SQL](https://img.shields.io/badge/T--SQL-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Oracle SQL](https://img.shields.io/badge/Oracle_SQL-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![MS Fabric](https://img.shields.io/badge/Microsoft_Fabric-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Fabric Pipelines](https://img.shields.io/badge/Fabric_Pipelines-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

**BI & Visualisation**

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Qlik Sense](https://img.shields.io/badge/Qlik_Sense-009848?style=for-the-badge&logo=qlik&logoColor=white)
![Fabric Notebooks](https://img.shields.io/badge/Fabric_Notebooks-0078D4?style=for-the-badge&logo=jupyter&logoColor=white)

**Currently Learning**

![Deneb](https://img.shields.io/badge/Deneb_(Vega--Lite)-1F3F5B?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![D3.js](https://img.shields.io/badge/D3.js-F9A03C?style=for-the-badge&logo=d3dotjs&logoColor=white)
![Custom SVG Visuals](https://img.shields.io/badge/Custom_SVG_Visuals-FFB400?style=for-the-badge)

---

## 👨‍💻 About me, in code

```python
from pyspark.sql import SparkSession
from pyspark.sql.functions import lit, concat

spark = SparkSession.builder.appName("Irinel").getOrCreate()

me = spark.createDataFrame([{
    "name":     "Irinel Cristea",
    "role":     "Analytics Engineer",
    "stack":    "MS Fabric · Power BI · PySpark · SQL",
    "based_in": "Cluj-Napoca, Romania",
    "building": "pipelines by day, weird charts by night",
    "motto":    "if the data is clean, anything is possible"
}])

me.select(
    concat(
        lit("Hi, I'm "), me.name,
        lit(" — a "), me.role,
        lit(" based in "), me.based_in, lit(".\n"),
        lit("I work with "), me.stack, lit(".\n"),
        lit("Currently "), me.building, lit(".\n"),
        lit("I believe: '"), me.motto, lit("'")
    ).alias("introduction")
).show(truncate=False)
```

```
+-----------------------------------------------------------------------------------------------+
| introduction                                                                                  |
+-----------------------------------------------------------------------------------------------+
| Hi, I'm Irinel Cristea — a Analytics Engineer based in Cluj-Napoca, Romania.                 |
| I work with MS Fabric · Power BI · PySpark · SQL.                                            |
| Currently building pipelines by day, weird charts by night.                                  |
| I believe: 'if the data is clean, anything is possible'                                      |
+-----------------------------------------------------------------------------------------------+
```

---

## 📬 Get in touch

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/irinel-cristea/)
[![Medium](https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@irinelcristea)
[![Twitter / X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/CristeaIrinel)
