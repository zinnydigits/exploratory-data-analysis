### Project Overview
The project aims to analyze the performance of a digital campaign by examining key metrics like conversion rates, total users gained, bounce rates, and most effective channels. Through thorough data analysis, insights were derived to optimize future campaign strategies and enhance overall marketing efficiencies.

![digitalcampaign_dashboard](https://github.com/zinnydigits/exploratory-data-analysis/blob/main/digital-campaign/digital-campaign-db.PNG)

### Data Source
The data was obtained from [absentdata.com](https://absentdata.com/data-analysis/where-to-find-data/).

### Tools
- **Microsoft Excel:** Used for data preprocessing and initial analysis.
- **Power Query:** Part of the Microsoft Power BI suite, Power Query was used for data cleaning, transformation, and integration.
- **Power BI for Visualization:** Power BI, a data visualization tool that enables the creation of interactive dashboards and reports was used to visualize the analyzed data in a clear and insightful manner.

### DAX Formula
```  Total Conversion =
                        IF (SUM(full_web[Conversions]) >= 1000,
                        FORMAT(SUM(full_web[Conversions])/1000, "0.00") & "K",
                        FORMAT(SUM(full_web[Conversions]), "0"))
```

### Visualization
- **Bar Charts:** Visualize channel conversions.
- **Treemap Chart:** Display bounce rates by channel.
- **Funnel Charts:** Compare total sessions to total conversions.
- **Line Charts:** Show monthly trends for average sessions and conversions.
- **Donut Chart:** Represent total users by channel.


### Explanatory Data Analysis
- Majority of the users, roughly 91%, are Organic Searchers.
- The highest average bouncing sessions were from Other Channels.
- The peak session occurred in September.
- 1.4% of Sessions were conversions
- The highest conversion rate was in March, slightly above May.
- The channels had comparable conversion rates.

### Recommendation
- Efforts should be made to attract users from paid channels.
- Page optimization is crucial to reduce bounce rates from other channels.
- Organic growth of the page is encouraged.

### References
- [absentdata.com](https://absentdata.com)
- Chandoo Youtube Channel

Note: This repository also contains the [raw data](https://github.com/zinnydigits/exploratory-data-analysis/blob/main/digital-campaign/digital_campaign_Data.xlsx), [cleaned data](https://github.com/zinnydigits/exploratory-data-analysis/blob/main/digital-campaign/cleaned_digital_campaign_Data.xlsx) and [power BI](https://github.com/zinnydigits/exploratory-data-analysis/blob/main/digital-campaign/digital_campaign_dashboard.pbix) file of this project.
