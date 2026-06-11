# Shein-Product-Funnel-Analysis
# 🧠 E-Commerce Pricing Funnel Analysis (SHEIN Dataset)

## 📌 Overview
This project analyzes **pricing strategies in an e-commerce dataset (SHEIN)** using a **funnel-based approach**.

The objective is to track how products move across pricing stages and identify drop-offs that may impact product visibility and potential conversions.

The analysis is further extended through segmentation by **category**, **color**, and **size** to uncover deeper pricing and inventory patterns.

---

## 🎯 Objectives

- Build a pricing funnel across product lifecycle stages
- Identify key drop-offs and inefficiencies in discount strategies
- Perform segmented analysis by category, color, and size
- Generate actionable business insights

---

## 🗂️ Dataset

- 📦 **~1,000 products**

### Features

| Feature | Description |
|----------|------------|
| `initial_price` | Original product price |
| `final_price` | Discounted selling price |
| `discount` | Discount percentage |
| `category` | Product category |
| `color` | Product color |
| `size` | Available size |
| `in_stock` | Inventory availability |

---

## ⚙️ Tech Stack

- **Python**
  - Pandas
  - NumPy
- **Visualization**
  - Plotly
  - Matplotlib
- **Environment**
  - Jupyter Notebook
  - Google Colab

---

## 🔄 Methodology

### 1. Data Cleaning

- Handled missing values
- Standardized the `in_stock` column
- Ensured pricing consistency

---

### 2. Funnel Definition

| Stage | Condition |
|---------|-----------|
| All Products | Full dataset |
| Discounted | `final_price < initial_price` |
| High Discount | `discount ≥ 30%` |
| In Stock | Available inventory |

> ✅ Each stage is sequentially filtered from the previous stage.

---

### 3. Funnel Results

| Stage | Count | Conversion % |
|---------|-------:|-------------:|
| All Products | 1000 | 100% |
| Discounted | 609 | 60.9% |
| High Discount | 107 | 10.7% |
| In Stock | 107 | 10.7% |

---

## 📊 Visualization

### 🔻 Pricing Funnel Chart

<p align="center">
  <img width="1739" height="469"
  src="https://github.com/user-attachments/assets/47576379-5759-4b9f-a038-75499751752e"
  alt="Pricing Funnel">
</p>

---

## 📉 Conversion Drop-Off

**Major Drop:** Discounted → High Discount (**~82% decrease**)

This indicates a limited availability of highly discounted products.

---

## 🔍 Segmented Analysis

The pricing funnel was extended across:

- 🧥 **Category** → Apparel, Accessories, etc.
- 🎨 **Color** → Discount distribution across colors
- 📏 **Size** → Relationship between inventory and discounts

---

## 💡 Key Insights

- Approximately **61%** of products are discounted.
- Only **18%** of discounted products qualify as high-discount items.
- The largest bottleneck occurs between the **Discounted → High Discount** stage.
- All high-discount products remain in stock, suggesting inventory is **not** the limiting factor.

---

## 📈 Business Impact

- Increase the proportion of high-discount products.
- Improve visibility of discounted items.
- Optimize pricing strategies at the category level.

---

## 🚀 Future Improvements

- 📅 Time-series analysis for seasonality trends
- 💰 Integration of sales data for a true conversion funnel
- 📊 Interactive dashboard using Tableau or Power BI
- 🤖 Machine learning-based price optimization

---

## ▶️ How to Run

```bash
pip install pandas numpy matplotlib plotly
```

Run the notebook:

```bash
jupyter notebook
```

or open the project in **Google Colab**.

---

## 📌 Project Outcome

This analysis demonstrates how funnel analytics can be applied beyond marketing to understand pricing behavior, inventory availability, and opportunities for improving product performance in e-commerce.
