# 💰 Mutual Fund Plan with Python

## 📘 Project Overview
The **Mutual Fund Plan with Python** project is a data-driven financial analysis built using **real Nifty 50 stock data**.  
The goal was to create a **mutual fund–style investment strategy** that offers **high returns with low risk** by analyzing volatility, ROI, and growth patterns of leading Indian companies.

This project demonstrates how Python can be used to design and evaluate a mutual fund portfolio using data analysis, visualization, and simulation techniques.

---

## 🎯 Objectives
- Identify companies with **high ROI** and **low volatility** from Nifty 50 data.  
- Construct a **balanced mutual fund portfolio** using inverse-volatility weighting.  
- Simulate **Systematic Investment Plans (SIPs)** to estimate long-term returns.  
- Visualize portfolio growth, risk-return relationships, and performance over time.  
- Help investors make **data-backed investment decisions**.

---

## ⚙️ Tools & Technologies
| Category | Tools Used |
|-----------|------------|
| Programming | Python |
| Libraries | Pandas, NumPy, Plotly, Matplotlib |
| Environment | Google Colab |
| Data Source | Nifty 50 closing-price dataset (CSV) |
| Techniques | ROI Calculation, Volatility Analysis, Monte Carlo Simulation, Inverse Volatility Weighting |

---

## 🧹 Data Preparation
1. **Data Loading** – Imported Nifty 50 closing-price dataset.  
2. **Cleaning** – Converted `Date` column to DateTime, handled missing values, and removed duplicates.  
3. **Feature Engineering** – Calculated:
   - `Volatility` (std dev of prices) → risk  
   - `Growth Rate` (pct change %) → average price growth  
   - `ROI` ((final – initial)/initial × 100) → total return  

---

## 📊 Exploratory Data Analysis (EDA)
Performed quantitative and visual analysis using Plotly:

### 🔹 Top Performers
- High-ROI stocks: **Bajaj Finserv**, **Bajaj Auto**, **Tata Motors**  
- Low-volatility stable stocks: **Infosys**, **TCS**, **HDFC Bank**

### 🔹 Key Metrics Summary
| Metric | Range (Across Nifty 50) |
|--------|--------------------------|
| Average ROI | 12 – 18 % |
| Average Volatility | 8 – 15 % |
| Risk Threshold | Median Volatility ≈ 10 % |

---

## 💼 Portfolio Construction
Selected companies with:
- ROI > Median ROI  
- Volatility < Median Volatility  

Weighted each stock **inversely proportional to volatility**:  
> `Weight = (1 / Volatility) ÷ Σ(1 / Volatility)`

This gave higher allocation to stable companies such as Infosys, HDFC Bank, and Asian Paints — achieving diversification and lower overall risk.

---

## ⚖️ Risk vs Return Comparison
- **Growth Stocks** → High ROI (16 – 18 %), Volatility ≈ 15 – 18 %.  
- **Mutual Fund Stocks** → ROI ≈ 12 – 14 %, Volatility ≈ 8 – 10 %.  

✅ Result: **Balanced portfolio with steady long-term growth and reduced risk.**

---

## 💰 SIP Simulation (₹5 000 per month, +10 % annual increase)
| Duration | Future Value (₹) |
|-----------|-----------------|
| 1 Year |    64 000 |
| 3 Years | 1.42 L |
| 5 Years | 1.30 L |
| 10 Years | 7.29 L |

➡️ **Average ROI:** 13.2 %  
➡️ **Portfolio Type:** Moderately Aggressive  
➡️ **Goal:** Stable, long-term wealth creation through compounding.

---

## 📈 Visualizations
| Visualization | Description |
|----------------|-------------|
| 📉 **Stock Price Trends** | Line plot of all Nifty 50 companies’ closing prices. |
| ⚖️ **Risk vs Return Bar Chart** | Compares volatility and ROI between mutual-fund vs growth companies. |
| 🥧 **Portfolio Composition Pie Chart** | Shows allocation based on inverse volatility weights. |
| 📈 **Future Value Projection Line Graph** | SIP growth over 1, 3, 5, and 10 years. |

*(All charts created with Plotly for interactive analysis.)*

---

## 🧠 Insights
1. High returns usually come with high risk — but a **data-driven mix** of stable companies provides better long-term results.  
2. **Inverse-volatility weighting** reduces exposure to risky stocks without sacrificing growth.  
3. Monthly SIPs with annual increments significantly boost future value via **compounding**.  
4. The mutual-fund plan achieved ~13 % expected annual returns with moderate risk.

---

## 🧩 Business Value
- Helps investors **visualize future returns and risks before investing.**  
- Enables fund managers to allocate capital scientifically based on data.  
- Demonstrates how **Python-based analysis can replace manual portfolio design.**

---

## 📂 Project Structure
