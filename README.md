# Airbnb-Listings-Analysis
# 🏡 Airbnb Listings Analysis Dashboard (Power BI)

## 📌 Project Overview

This project focuses on analyzing Airbnb listing data to uncover key insights related to pricing, availability, host activity, and customer engagement. The dashboard is built using Power BI and helps in understanding trends that can support business decisions.

---

## 🎯 Objectives

* Analyze listing availability and identify inactive listings
* Understand pricing distribution across locations
* Identify top-performing hosts and areas
* Explore customer engagement using reviews

---

## 🛠️ Tools & Technologies

* **Power BI** – Data visualization and dashboard creation
* **MySQL** – Data storage and querying
* **Excel/CSV** – Data source and preprocessing
* **DAX** – Measures and calculations

---

## 📊 Key Features

### 🔹 KPI Metrics

* Total Listings
* Active Listings
* Inactive Listings (availability < 1)
* % Inactive Listings
* Average Price
* Total Reviews

### 🔹 Dashboard Insights

* Listings distribution by neighbourhood
* Price variation across locations
* Availability trends over time
* Host performance analysis

---

## 🧮 Sample DAX Measure

```DAX
Inactive Listings = 
CALCULATE(
    COUNTROWS(airbnb_listings),
    airbnb_listings[availability_365] < 1
)
```

---

## 📂 Dataset Details

* Contains Airbnb listing data including:

  * Listing ID, Host details
  * Location (latitude, longitude, neighbourhood)
  * Price, service fee
  * Availability (365 days)
  * Reviews and ratings

---

## ⚙️ Data Cleaning Steps

* Removed blank rows and null values
* Handled data type conversions (dates, boolean)
* Removed duplicate records using SQL
* Standardized column formats

---

## 🚀 How to Use

1. Download the `.pbix` file from this repository
2. Open it in Power BI Desktop
3. Refresh data if needed
4. Explore the dashboard visuals

---

## 💡 Key Insights

* Identified inactive listings with zero availability
* Highlighted high-demand neighbourhoods
* Found variation in pricing based on location and room type
* Analyzed host activity and listing distribution

---

## 📈 Future Improvements

* Add time-series forecasting
* Integrate real-time data
* Enhance dashboard interactivity
* Deploy using Power BI Service

---

## 🤝 Contribution

Feel free to fork this repository and suggest improvements.

---

## 📬 Contact

If you have any questions or feedback, feel free to connect with me on LinkedIn.
