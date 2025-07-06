# 🏙️ Dubai Real Estate Intelligence Dashboard

This Power BI project explores housing trends across Urban, Suburb, and Rural neighborhoods in Dubai using a real-world dataset. The dashboard enables investors and real estate professionals to evaluate property characteristics like price, size, age, and bedroom configurations through an interactive interface.

---

## 🎯 Objective

The goal of this project is to design a professional and insightful Power BI dashboard that:

- Helps users compare housing prices and size across Dubai’s neighborhoods
- Analyzes construction age and bedroom mix trends
- Enables basic interactivity for data exploration
- Presents insights in a clean and storytelling-focused layout

---

## 🧾 Dataset Overview

The dataset includes 6 key columns:

| Column         | Description                            |
|----------------|----------------------------------------|
| `SquareFeet`   | Size of the property in sqft           |
| `Bedrooms`     | Number of bedrooms                     |
| `Bathrooms`    | Number of bathrooms                    |
| `Neighborhood` | Urban, Suburb, or Rural location tag   |
| `YearBuilt`    | Year when the property was built       |
| `Price`        | Selling price of the property (AED)    |

---

## 🔧 Data Preparation (Power Query)

Performed the following data cleaning steps:

- Removed nulls and duplicates
- Trimmed text and ensured consistent formatting
- Converted data types to appropriate formats (numeric/text)

### 🧠 Calculated Columns (DAX)

| New Column          | Description                                               |
|---------------------|-----------------------------------------------------------|
| `Price per SqFt`    | `Price / SquareFeet` — normalized value per unit area     |
| `Property Age`      | `2025 - YearBuilt` — construction age of property         |
| `Listing Category`  | Categorized as Budget, Mid-Range, or High-End using price percentiles |

---

## 📊 Dashboard Pages

### 📌 Page 1: Housing Analytics

| Section           | Description |
|-------------------|-------------|
| **KPI Cards**     | Total Listings, Avg Price, Max Price, Avg Size, Price per SqFt |
| **Bar Chart**     | Average Price by Neighborhood |
| **Stacked Column**| Bedroom Count by Neighborhood |
| **Treemap**       | Neighborhood-wise property count |
| **Scatter Plot**  | Price vs Size (SqFt) colored by Listing Category |
| **Property Age Bar** | Aggregated Age distribution across Neighborhoods |
| **Slicers**       | Bedrooms, Bathrooms, Neighborhood |


---

### 📌 Page 2: Executive Overview

| Section               | Description |
|------------------------|-------------|
| **Headline KPI**       | Total Market Value (Sum of Price) |
| **Line Chart**         | Price vs Size Trend |
| **Decomposition Tree** | Drill-down through Neighborhood ➜ Bedrooms ➜ YearBuilt ➜ Size |
| **Back Button**        | Navigation to return to main dashboard |


---

## 🔍 Key Business Questions Addressed

- What are the most expensive neighborhoods by average price?
- Which bedroom types dominate the Dubai housing market?
- How does property age vary by neighborhood?
- How does size influence price across listing categories?

---

## 💡 Insights

- 🏡 **Rural properties have the highest average prices**, likely due to larger villa-style homes.
- 📏 **Price increases exponentially with size**, especially above 2500 sqft.
- 🛏 **3-bedroom homes dominate Mid-Range segments**, suggesting affordability preferences.
- 🧱 Most homes are between **15 to 40 years old**, with the oldest from 1950.
- 📍 Suburb areas show **balanced distributions** across Budget to High-End listings.

---

## 📁 Project Structure

<pre> ## 📁 Project Structure ``` dubai-housing-dashboard/ ├── data/ │ └── housing_price_dataset.csv ├── screenshots/ │ ├── page 1 - housing analytics.png │ └── page 2 - executive summary.png ├── DUBAI HOUSING DASHBOARD Insights.docx ├── DubaiHousingPrices.pbix └── README.md ``` </pre>

---

## 🛠 Tools Used

- **Power BI Desktop**
- **Power Query Editor**
- **DAX (Data Analysis Expressions)**

---

## ✅ Final Notes

This dashboard delivers both a visual storytelling experience and practical insights for real estate decision-making. With clearly segmented pages and smart metrics, it meets the expectations outlined in the assignment while remaining clean, interactive, and insightful.
