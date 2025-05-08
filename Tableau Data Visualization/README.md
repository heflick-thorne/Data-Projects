# 📊 Superstore Profitability and Operations Analysis

This project analyzes a fictional superstore's sales and returns data to identify key profit drivers, evaluate advertising opportunities, and investigate return behaviors. The goal is to deliver actionable insights through data visualizations using tools such as Tableau (or another BI tool).

---

## 🧩 Part 1: Profit & Loss Analysis

To begin, I explored combinations of dimensions (e.g., Sub-Category + Region, Shipping Mode + Product ID) to identify:

- **Top 2 profit-generating segments**
- **Top 2 loss-making segments**

Visualizations were created to support these findings, highlighting which combinations brought consistent profits and which drained revenue.

Next, I identified:
- **Individual products that consistently generate losses**  
- **Three product subcategories to prioritize**  
- **Three product subcategories to phase out**  

Each recommendation is supported with visual evidence based on aggregated profit metrics.

---

## 📢 Part 2: Advertising Strategy

To determine if advertising would be cost-effective, I analyzed **monthly profit trends across U.S. states**. I identified:

- **Top 3 state + month combinations** for ad targeting based on average monthly profit.
- Developed a **visualization of average monthly profit** for these states to highlight seasonality.

Assuming a 20% ad spend budget (i.e., spend up to 1/5 of profits), I calculated how much the store should invest in ads for each high-return month/state combination.

---

## 🔄 Part 3: Returns Analysis

I incorporated the **Returns table** by creating a calculated field that converts:
- `"Yes"` → `1`
- `null` → `0`

Using this binary return indicator, I visualized:
- **Products with the highest return rates**
- **Customers with the highest return rates**

Additionally, I built a visualization plotting **average profit vs. average return rate** across a selected dimension (e.g., Product Type, Shipping Mode, or State). This visual argument supports whether the store should continue operating in specific categories or reconsider its strategy.

---



