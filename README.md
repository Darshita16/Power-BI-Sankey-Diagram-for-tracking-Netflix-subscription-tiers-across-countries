# 📊 Power BI Sankey Diagram: Telco Customer Churn Flow

This project uses a **Sankey diagram** in Power BI to visualize the **customer churn flow** in a telecom dataset. The goal is to uncover how customers transition across different stages—**from active or churned status**, through **churn labels**, to **churn categories and reasons**.

---

## 📌 Project Overview

Customer churn is a critical challenge in the telecom industry. By using Power BI's Sankey chart, we can visualize:

- The number of customers who churned vs. remained active
- The category and reason for churn
- Flow insights for better retention strategies

---

## 🔧 Tools Used

- **Power BI Desktop**
- **Power Query Editor**
- **Sankey Chart by Microsoft or OKViz** (Power BI Visual)

---

## 📁 Dataset

- Source: `telco.csv` (Telecom Customer Data)
- Key columns used:
  - `Customer Status`
  - `Churn Label`
  - `Churn Category`
  - `Churn Reason`

---

## 🔁 Data Transformation Steps

The dataset was processed in Power Query to form a multi-step flow:

1. **Customer Status ➡ Churn Label**
2. **Churn Label ➡ Churn Category**
3. **Churn Category ➡ Churn Reason**

Each pair was:
- Grouped
- Counted
- Standardized into `Source`, `Destination`, and `Count` columns

All flows were appended into a master table for visualization.

---

## 📊 Visualization

A Sankey diagram was created using the following configuration:

- **Source**: Stage (Status/Label/Category)
- **Destination**: Next stage in the flow
- **Weight**: Count of customers

This reveals how and why customers drop off at different stages of their lifecycle.

---

## 🧠 Insights

- Majority of churned customers left due to **competitive offers** and **limited service quality**
- **Dissatisfaction and price-related issues** were common among long-term churners
- The Sankey diagram effectively traced the most frequent churn pathways

---

## 🚀 How to Use

1. Open Power BI Desktop
2. Load the `telco.csv` dataset
3. Use Power Query to transform the dataset as described
4. Add the **Sankey Chart** from AppSource
5. Map `Source`, `Destination`, and `Count` to the visual

---

## 📂 Folder Structure


