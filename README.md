# 🍽️ Zomato Bangalore Restaurants - Exploratory Data Analysis (EDA)

An end-to-end Exploratory Data Analysis (EDA) and data cleaning project on the Zomato Bangalore restaurant dataset containing over 51,000 records.

## 📌 Project Overview
This project focuses on cleaning unstructured restaurant data, handling missing/dirty entries, aggregating low-frequency categorical features, and extracting business insights on restaurant ratings, delivery availability, table booking, and neighborhood trends.

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## 🧹 Data Cleaning & Preprocessing Steps
1. **Feature Selection:** Dropped redundant and high-cardinality metadata (`url`, `address`, `phone`, `menu_item`, `dish_liked`, `reviews_list`).
2. **Handling Duplicates:** Removed duplicate restaurant listings to ensure data integrity.
3. **Rating Transformation:**
   - Stripped `/5` formatting and non-numeric entries (`NEW`, `-`).
   - Imputed missing ratings using column mean values.
4. **Cost Parsing:** Cleaned comma separators from `approx_cost(for two people)` and cast to numerical float.
5. **Category Binning:**
   - Grouped rare restaurant types (<1000 count) into `'others'`.
   - Grouped low-frequency locations (<300 count) and cuisines (<100 count) into `'others'`.

## 📊 Key Visualizations & Insights
* **Location Distribution:** Identified top restaurant hubs across Bangalore (e.g., BTM, HSR, Koramangala).
* **Delivery & Booking Trends:** Compared rating distributions across restaurants offering online ordering vs. offline-only setups.
* **Price vs. Ratings:** Analyzed the correlation between dining costs and customer ratings.

## 🚀 How to Run Locally
1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/zomato-restaurant-eda.git# zomato-restaurant-eda
Description: Exploratory Data Analysis (EDA) and data cleaning on the Zomato Bangalore Restaurants dataset using Python, Pandas, Matplotlib, and Seaborn.
