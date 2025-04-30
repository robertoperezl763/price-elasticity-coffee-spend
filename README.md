# ☕️ Price Elasticity and Customer Spend Modeling for a Coffee Chain

## 📌 Problem Statement:
What factors infleunce how much consumers spend each mont? How sensitive are customers to changes in pricing?
Are we missing insights by only looking at the customers who entroll?

---

## 🔍  Tehcniques Used
- **Log-log regression** (elasicity modeling)
- **Heckman 2-step regression** (to correct for selection bias in data)
- **Exploratory Data Analysis** and **Data Visualization**
- **Business impact analysis** based on model predictions

---

## 📊  Key Findings
- A **1% increase** in average drink price leads to a **1.775% decrease** in spend
- **Female customers** spend **~7x more** per month than male customers
- Each additional **year of age** leads to **~1.01%** increase to customer monthly spend
- Correcting for selection bias in data reveealed that the **price sensitivity** was hihger than initially estimated

--- 

## 💡  Business Impact
Reducing average drink prices from the current average of **$6 to $5** could generate an estimated **$3.2 billion** in extra global revenue per month
Female customers represent a **high-value customer demographic** - suggesting a *targeted marketing opportunity*

---

## 📂  Repo Structure
```
📁 coffee-pricing-elasticity/
├── README.md  
├── 📁 [data](https://github.com/robertoperezl763/price-elasticity-coffee-spend/tree/main/data)/  
│   └── README_data.md  
├── 📁 [workfile](https://github.com/robertoperezl763/price-elasticity-coffee-spend/tree/main/workfile)/  
│   └── price_elasticity_coffee.Rmd  
├── 📁 [visuals](https://github.com/robertoperezl763/price-elasticity-coffee-spend/tree/main/visuals)/  
│   ├── loglog_model.png  
│   ├── heckmanTwoStep_model.png  
│   ├── maleVFemale_plot.png  
│   └── predictedMonthlySpend_plot.png  
├── 📁 [report](https://github.com/robertoperezl763/price-elasticity-coffee-spend/tree/main/report)/  
│   ├── price_elasticity_coffee.pdf  
│   └── price_elasticity_coffee.html  
└── .gitignore
```



## 🧭  Possible Next Steps
- Explore time series trends (e.g., monthly seasonality)
- Incorporate regional pricing variation
- Simulate pricing strategies under specific constraints (e.g., cost, competition)

---

## 📌 Disclaimer

This dataset is **simulated** and was provided as part of a university course project. It does **not** contain real customer data, and any resemblance to real individuals or businesses is purely coincidental. The data is being used solely for educational and demonstration purposes.


## 👤  Author
Created by Roberto Perez Lopez\
[LinkedIn](https://www.linkedin.com/in/roberto-perezl/) | [GitHub](https://github.com/robertoperezl763/) | [Email](mailto:robertoperezl761@gmail.com)
