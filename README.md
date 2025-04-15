# 🪐 Mars Web Scraping & Weather Data Analysis #

## 🚀 Overview

This project is part of a data science challenge focused on **web scraping, data cleaning, and analysis** using Python. The objective is to scrape data from static Mars-related web pages and perform meaningful analysis and visualization to extract insights.

The challenge is split into two main parts:

- **Deliverable 1:** Scrape Mars news articles (titles and preview texts).
- **Deliverable 2:** Scrape and analyze Mars weather data, including temperature and atmospheric pressure patterns.

---

## 🔧 Tools & Technologies

- Python   
- Jupyter Notebook  
- [Splinter](https://splinter.readthedocs.io/en/latest/) – for browser automation  
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) – for HTML parsing  
- [Pandas](https://pandas.pydata.org/) – for data manipulation  
- [Matplotlib](https://matplotlib.org/) – for visualizations  

---

## 📂 Project Structure

| File                         | Description                                                                 |
|------------------------------|-----------------------------------------------------------------------------|
| `part_1_mars_news.ipynb`     | Scrapes news titles and previews from a static Mars News site.             |
| `part_2_mars_weather.ipynb`  | Scrapes Mars weather data, processes it, and performs analysis/visualizations. |
| `mars_weather.csv`           | Exported CSV containing cleaned Mars weather data.                         |
| `output.png`                 | Visualization of minimum temperature trends used to estimate Martian year. |
| `README.md`                  | Project documentation and analysis summary.                                |

---

## 📰 Part 1: Mars News Scraping

### ✔️ Data Source:
- Static site: [Mars News](https://static.bc-edx.com/data/web/mars_news/index.html)

### ✔️ Task:
- Use Splinter and BeautifulSoup to extract:
  - **Title** of each news article
  - **Preview** text of each article
- Store each record as a dictionary:
  ```python
  {
      "title": "NASA’s Perseverance Rover Investigates Geologically Rich Mars Terrain",
      "preview": "The rover’s robotic arm is examining rocks in an ancient river delta."
  }

## 🌡️ Part 2: Mars Weather Data Scraping & Analysis
✔️ Data Source:
Static site: Mars Weather Table

✔️ Task:
Extract tabular data using BeautifulSoup.

Create a Pandas DataFrame with columns:

id, terrestrial_date, sol, ls, month, min_temp, pressure

Convert data types:

terrestrial_date → datetime

sol, ls, month → int

min_temp, pressure → float

## 📊 Data Analysis & Visualizations
🌡️ Minimum Temperature
Coldest Month: Month 3

Warmest Month: Month 8

A bar chart was created showing average minimum temperature by month, sorted from coldest to warmest.

🌀 Atmospheric Pressure
Lowest Pressure: Month 9

Highest Pressure: Month 6

Pressure trends were visualized in a bar chart grouped by month.

📆 Martian Year Estimation
By plotting minimum daily temperatures over Earth dates, a cyclical seasonal pattern was observed.

Estimated Martian year length: ~687 Earth days, based on repeated temperature patterns over time.

📤 Exported Output
Cleaned Mars weather data saved as: mars_weather.csv

Line chart of minimum temperatures over time saved as: output.png

📈 Example Visuals
✅ Average Minimum Temperature by Month (Sorted)

✅ Average Atmospheric Pressure by Month

✅ Temperature Over Time to Estimate Martian Year

## 🧠 Key Learnings
Gained hands-on experience with web scraping from static HTML.

Practiced browser automation using Splinter.

Reinforced Pandas skills for cleaning, grouping, and analyzing data.

Visualized real-world Martian climate patterns and interpreted seasonal changes.

## 🗂️ Credits
Mars News and Weather data provided by Berkeley Data Science Boot Camp - EdX

Developed as part of a data analytics learning challenge.

