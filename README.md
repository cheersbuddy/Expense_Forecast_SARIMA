# 📊 Expense Forecast Summary (SARIMA)

This document provides a structured summary of forecasted expenses using SARIMA models, with breakdowns across different time horizons. The forecasts are based on historical patterns and aim to support strategic financial planning.

---

## 🔍 Forecast Summary by Time Period

### 📅 Monthly Forecast
| Period       | Forecasted Value | Actual Value | Difference | Accuracy  |
|--------------|------------------|--------------|------------|-----------|
| March 2025   | ₹33,524.35     | ₹32,383.08   | ₹1,141.27   | 96.48%    |

### 🗓️ Quarterly Forecast
| Period       | Forecasted Value | Actual Value | Difference | Accuracy  |
|--------------|------------------|--------------|------------|-----------|
| Q1 2025      | ₹2,661,032.91  | ₹2,658,815.98 | ₹2,216.93   | 99.92%    |

### 📆 Half-Yearly Forecast
- **Model Used:** SARIMA (Order: (0, 2, 0), Seasonal Order: (0, 2, 1, 2))
- **Forecasted Value:** ₹3,453,612.27  
- **Actual Value:** ₹3,377,654.58  
- **Difference:** ₹75,957.69  
- **Accuracy:** 97.75%

### 📈 Yearly Forecast
| Period       | Forecasted Value | Actual Value | Difference | Accuracy  |
|--------------|------------------|--------------|------------|-----------|
| 2025         | ₹3,242,190.48  | ₹3,661,628.47 | ₹419,437.99 | 88.55%    |

---

## 📌 Forecast Selection Logic

**Users can select forecast periods based on the current date. Options are dynamically limited as follows:**

### 🗓️ Period Filters:
- **Month:** Only current and next month available for selection.
- **Quarter:** Only current and next quarter available.
- **Half-Year:** Only current and next half-year.
- **Annual:** Only current and next financial year.

> **Note:** Quarter, half-year, and annual ranges are based on the company's official financial year.

### 🔄 Forecast Calculation Rule:
- Forecasts are based on the pattern of existing data.
- For a selected period `P`, the model considers data up to `(P + 2 * previous period)` to enhance accuracy.

---

## 📊 Visual Insights & Interpretations

### 1. **Net Expense + 3-Month Rolling Mean**
![image](https://github.com/user-attachments/assets/4bf6e51b-ac45-480d-b605-00c66d8119d6)

**What it shows:**
- Actual monthly expenses vs. a smoothed trend using a 3-month rolling mean.

**Why it's useful:**
- Highlights anomalies like sudden spikes or drops.
- Removes short-term noise, improving long-term trend visibility.

**Business Example:**
> "Why was February 2024's expense 3x the average? Was it an annual license fee? Should we budget for this next year?"

---

### 2. **Transaction Volume Over Time**
![image](https://github.com/user-attachments/assets/846dce8b-d91f-4b67-8f50-fdf547f739df)

**What it shows:**
- Number of transactions each month.

**Why it's useful:**
- Distinguishes between large one-time costs and many small transactions.
- Helps identify inefficiencies or potential fraud.

**Business Example:**
> "April had the same expense as March, but 3x the number of transactions. Are purchases being split unnecessarily?"

---

### 3. **Rolling Standard Deviation (Volatility)**
![image](https://github.com/user-attachments/assets/04f52f46-0c06-4e7d-99ef-2c4048af2e8f)

**What it shows:**
- The fluctuation level in monthly expenses.

**Why it's useful:**
- Evaluates expense predictability.
- Departments with high volatility may need tighter budgeting or contingency funds.

**Business Example:**
> "HR department expenses are unpredictable. Should we enforce a cap or allocate buffer budgets?"

---

## ✅ Key Takeaways
- SARIMA models offer accurate short- to long-term expense forecasting.
- Period filters ensure practical, time-relevant forecasts.
- Visual tools provide actionable insights for finance and operations teams.
- Forecasts help preempt budget issues and plan strategically based on past patterns.

---

_This documentation is intended to support analysts, finance teams, and decision-makers in interpreting and applying forecasted financial data._

