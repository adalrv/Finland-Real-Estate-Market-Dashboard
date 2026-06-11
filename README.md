# 🇫🇮 Finland Real Estate Market Dashboard

An end-to-end data analytics project that scrapes, cleans, and visualizes the Finnish residential housing market using **Python (Web Scraper)** and **Tableau**. 

## 🎯 Project Overview
This repository contains a dynamic **Tableau Dashboard** designed to analyze property listings across Finland. The project bridges the gap between raw web data and actionable real estate insights, allowing users to explore prices, locations, and property characteristics seamlessly.

## 📊 Dashboard Preview
![Tableau Dashboard Preview](image_1fc03e.png)

## ❓ Problem Statement
Finding housing or analyzing real estate investment opportunities in Finland can be challenging due to decentralized information across various listing platforms. 

* 🚫 **Lack of Centralized Insights:** Data is often fragmented, making it hard to see country-wide trends.
* 📉 **Hidden Market Dynamics:** Vital metrics like the average price per square meter (`€/m²`) across different municipalities are not easily comparable at a glance.
* ⏱️ **Manual Effort:** Investors and buyers spend hours manually comparing properties without a data-driven benchmark.

## 🌐 Data Source & Engineering (Origen de Datos)
The data used in this project was built entirely from scratch through an automated pipeline:

* 🕷️ **Web Scraping:** Developed a custom Python web scraper to extract real-time data from primary Finnish real estate portals using `Data Real Estate Finland.xlsx`.
* 📋 **Dataset Details:** Gathered **702 unique residential listings** containing 40 structural attributes (e.g., price, area, building year, room count, sauna availability, and precise geographical coordinates).
* 🛠️ **Data Extraction & Joining:** Extracted missing geographic hierarchies by joining regional data tables to map out municipalities directly into their respective Finnish regions (`Maakunnat`).
* 🧹 **Data Cleaning:** Handled missing values (specifically in the `totalArea` and `buildYear` variables), converted raw currency strings into numeric fields, and filtered out non-residential listings.

## 🔍 Data Analysis & Key Insights
Based on the exploratory data analysis (EDA) of the scraped market snapshot:

* 📈 **Market Distribution:** The capital region concentrates the highest density of online listings, with **Helsinki (85)**, **Espoo (47)**, and **Vantaa (32)** representing a massive share of the market, alongside major regional hubs like **Kuopio (51)** and **Oulu (44)**.
* 💶 **Price Disparities:** The average residential property price in the dataset sits around **€209,983**, with high-end luxury properties peaking up to **€1.54M**.
* 📏 **The Square Meter (`€/m²`) Premium:** 
  * **Helsinki** commands the highest premium at an average of **~€4,678/m²**.
  * **Espoo** follows closely at **~€3,730/m²**, and **Vantaa** at **~€3,170/m²**.
  * Northern and Central hubs offer significantly more space per Euro, with **Oulu (~€2,518/m²)** and **Kuopio (~€2,247/m²)** displaying much higher affordability.
* 🏡 **Property Profiles:** The average size of a listed residential property is **107 m²**, spanning a broad range from compact city studios (19 m²) to large detached family homes (600 m²).

## 💡 Conclusions
* 🔑 **Location is the Primary Driver:** The capital region (Helsinki-Espoo-Vantaa) shows a clear price premium that detaches itself from the rest of the country's average square meter valuation.
* 🏗️ **Data-Driven Decisions:** Transitioning from raw web tables to a visual map-based Tableau interface enables instant filtering of properties based on specific criteria like *Price per m²* or *Sauna presence*, empowering buyers to spot undervalued deals.
* 🔄 **Scalability:** The architecture of the Python scraper allows this dashboard to be updated periodically, creating a historical timeline of price fluctuations in the Finnish housing market.

## 🛠️ Tech Stack & Tools
* **Language:** Python 🐍 (BeautifulSoup / Scrapy, Pandas, NumPy)
* **Visualization:** Tableau Desktop / Public 📊
* **Data Format:** Excel / CSV 📁

## 🚀 How to Interact with the Dashboard
1. Clone this repository or download the dataset.
2. Open the `.twbx` file using Tableau Desktop or Tableau Public.
3. Use the interactive filters on the left panel to filter by **City**, **Property Type**, or **Price Range**.

---
*Developed by Adalberto Rosendo Vargas* 🚀
