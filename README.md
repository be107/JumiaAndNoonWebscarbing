# 📺 TV Products Web Scraping – Jumia & Noon

## 📌 Project Overview

This project focuses on collecting and preparing television product data from two major Egyptian e-commerce platforms: **Jumia Egypt** and **Noon Egypt**.

Using Python and Selenium, product information was extracted from both websites, combined into a single dataset, and cleaned using Pandas to produce a structured CSV file ready for further analysis.

## 🎯 Project Objectives

- Automate product data collection from multiple e-commerce websites.
- Extract TV product information, including prices, ratings, and reviews.
- Combine data from different sources into one dataset.
- Clean and standardize the collected data.
- Export the final dataset into CSV format.

## 🛠️ Technologies Used

- **Python** – Main programming language.
- **Selenium** – Browser automation and web scraping.
- **Pandas** – Data manipulation and cleaning.
- **Jupyter Notebook** – Development and execution environment.
- **Google Chrome / ChromeDriver** – Browser automation.

## 🌐 Data Sources

- [Jumia Egypt](https://www.jumia.com.eg/)
- [Noon Egypt](https://www.noon.com/egypt-en/)

## 📊 Data Collection

The scraper collects the following information for each TV product:

| Column | Description |
|---|---|
| `name` | Product name |
| `price_before_discount` | Original price |
| `price_after_discount` | Discounted price |
| `Rating` | Customer rating |
| `Reviews_count` | Number of customer reviews |
| `Link` | Product page URL |
| `image_url` | Product image URL |
| `Source` | E-commerce platform (Jumia or Noon) |

## ⚙️ Data Collection Process

1. Opened the product listing pages using Selenium WebDriver.
2. Navigated through multiple pages on both platforms.
3. Extracted product details using CSS selectors.
4. Stored the extracted information in Python dictionaries.
5. Combined the collected records into a Pandas DataFrame.
6. Exported the initial dataset to CSV.

## 🧹 Data Cleaning

The collected dataset went through several cleaning steps:

- Converted rating and review count columns into numeric formats.
- Handled missing values in ratings and review counts.
- Standardized price columns and converted them into numeric values.
- Removed records with incomplete rating/review information according to the applied cleaning rule.
- Identified and removed duplicate records.
- Exported the cleaned dataset into a CSV file.

## 📈 Project Results

| Metric | Result |
|---|---:|
| Initial records | 647 |
| Records after missing-value filtering | 615 |
| Duplicate records removed | 25 |
| Final cleaned records | **590** |
| Data sources | 2 |
| Final columns | 8 |

## 📁 Project Files

```text
JumiaAndNoonWebscarbing/
│
├── Tvs.ipynb
├── tvs.csv
└── tvs_cleaned.csv
```

- `Tvs.ipynb`: Contains the scraping and data-cleaning workflow.
- `tvs.csv`: Initial collected dataset.
- `tvs_cleaned.csv`: Final cleaned dataset.

*The CSV files are generated when the notebook is executed.*

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/be107/JumiaAndNoonWebscarbing.git
```

### 2. Install the required libraries

```bash
pip install selenium pandas jupyter
```

### 3. Set up ChromeDriver

Make sure Google Chrome and a compatible ChromeDriver are installed and accessible.

### 4. Run the notebook

Open `Tvs.ipynb` using Jupyter Notebook or VS Code and execute the cells.

## 💡 Key Skills Demonstrated

- Web Scraping & Browser Automation
- Selenium WebDriver
- HTML Element Inspection & CSS Selectors
- Data Extraction from Multiple Sources
- Data Cleaning & Preprocessing
- Handling Missing Values and Duplicates
- Data Type Conversion
- CSV Data Export

## ⚠️ Notes

- Product prices, ratings, and availability may change over time.
- Some products may not have customer ratings or review counts.
- Website structures and CSS selectors may change, requiring updates to the scraper.
- This project was developed for educational and portfolio purposes. Please respect the websites' terms of service and scraping policies.

---

**Developed by Habiba Hussam**

[GitHub Profile](https://github.com/be107)
