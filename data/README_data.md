## 📌 Disclaimer

This dataset is **simulated** and was provided as part of a university course project. It does **not** contain real customer data, and any resemblance to real individuals or businesses is purely coincidental. The data is being used solely for educational and demonstration purposes.


# 📁 Data Overview

This directory contains two datasets used for modeling customer spending and price sensitivity at a coffee chain. The datasets simulate customer survey data and transaction records tied to a rewards program.

---

## 🗂️ Dataset 1: `sbux_survey.txt`

**Description:**  
A simulated survey dataset with 10,000 observations capturing demographic information and whether a customer enrolled in the app-based rewards program.

**Columns:**
| Column Name        | Type     | Description                                                      |
|--------------------|----------|------------------------------------------------------------------|
| `id`               | `int`    | Unique identifier for each customer                              |
| `enroll`           | `int`    | Rewards program enrollment status (`1` = enrolled, `0` = not enrolled) |
| `age`              | `int`    | Age of the customer                                              |
| `female`           | `int`    | Gender indicator (`1` = female, `0` = not female)                |
| `enrollPromoValue` | `float`  | Dollar value of promotional incentive offered at enrollment      |

---

## 🗂️ Dataset 2: `sbux_transactions.txt`

**Description:**  
Contains spending and pricing data for the 3,077 customers who self enrolled in the rewards program. All customer IDs in this file appear in the survey dataset.

**Columns:**
| Column Name        | Type     | Description                                                      |
|--------------------|----------|------------------------------------------------------------------|
| `id`               | `int`    | Unique identifier for each customer                              |
| `monthlySpend`     | `float`  | Average monthly spend (in dollars)                               |
| `avgPrice`         | `float`  | Average price paid per coffee drink                              |
| `age`              | `int`    | Age of the customer                                              |
| `female`           | `int`    | Gender indicator (`1` = female, `0` = not female)                |
| `enrollPromoValue` | `float`  | Dollar value of promotional incentive offered at enrollment      |

---

## 🔗 Notes

- All records in `sbux_transactions.txt` are for users who **enrolled** in the rewards program (`enroll = 1` in `sbux_survey.txt`).
- Use the `id` column to **join** the two datasets.
- The survey dataset enables **correction for selection bias** using Heckman’s two-step regression.
- Gender and enrollment are represented as **binary integers** (`0` or `1`), not booleans.

---

## 📎 File Format

Both datasets are in **tab-delimited `.txt`** format.

