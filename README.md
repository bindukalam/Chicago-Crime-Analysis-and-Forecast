# 🏙️ Chicago Crime Analysis & Forecast

A data science project analyzing over **1 million crime records** from Chicago (2012–2016) 
to uncover patterns and forecast future crime trends using Facebook Prophet.

> **Course:** EAS503 – Programming Database for Data Scientists  
> **Team:** Sreerag Venugopalan, Nitin Chandra Goud Viltapuram, Bindu Kalam, Arun Sreevatsa Peddakotla

---

## 📌 Project Overview

With over **80.7% of the US population** living in urban areas, monitoring and predicting 
criminal activity has become critical for smart governance. This project uses Chicago's 
open crime dataset to identify patterns and build a forecasting model that can assist 
in intelligent policing decisions.

---

## 📂 Dataset

- **Source:** [Kaggle – Crimes in Chicago](https://www.kaggle.com/currie32/crimes-in-chicago)
- **Size:** 1.04 million records (2012–2016)
- **Columns:** 22 attributes including Date, Block, Primary Type, Location Description, 
  District, Ward, Arrest status, GPS Coordinates, and more

---

## 🗄️ Database Design

The dataset was normalized into a relational schema with 4 tables:

| Table | Description |
|-------|-------------|
| `IUCR` | Crime classification codes and types |
| `CRIME` | Core crime records with date, arrest status, FBI code |
| `ADDRESS` | Location details including coordinates and block info |
| `COMMUNITY` | District and ward-level groupings |

---

## 📊 Exploratory Data Analysis (EDA)

Key findings from the analysis:

- 📉 **Crime is decreasing** year over year — Chicago is becoming safer
- 📅 **1st of the month** records the highest crimes; last day records the least
- ❄️ **December** has the lowest crime rate across months
- 🔪 **Theft** (23.6K) is the most common crime type, followed by Battery and Criminal Damage
- 🛣️ Most crimes occur on **Streets** (23.7K), followed by Residences and Apartments
- 🏘️ **11th District (Harrison)** has the highest crime count by district

---

## 🔮 Crime Forecasting

Used **Facebook Prophet** — an open-source time series forecasting library by Meta's 
Core Data Science team — to predict crime trends.

### Forecast Results:
- A **negative trend** is predicted for 2017–2018, supporting the hypothesis that 
  Chicago is becoming progressively safer
- **Peak crime period:** March 1st – May 1st
- **Lowest crime period:** November 1st – March 1st

---

## 🛠️ Technologies Used

- **Python** – Core programming language
- **SQLite** – Relational database for normalized data storage
- **Facebook Prophet** – Time series forecasting
- **Pandas / Matplotlib** – Data manipulation and visualization

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `*.py` | Python scripts for EDA and forecasting |
| `Final_Project.pptx` | Full project presentation with visualizations |
| `README.md` | Project documentation |

---

## 📚 References

- [Chicago Crime Dataset – Kaggle](https://www.kaggle.com/currie32/crimes-in-chicago)
- [City of Chicago Open Data](https://data.cityofchicago.org/)
- [Facebook Prophet Documentation](https://facebook.github.io/prophet/docs/quick_start.html)
- [US Urban Population Stats](https://www.census.gov/programs-surveys/geography/guidance/geo-areas/urban-rural/ua-facts.html)
