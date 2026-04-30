# 🏦 Bank Loan Default Analysis Dashboard

An interactive **Power BI dashboard** analysing 255,347 bank loan records 
to identify default risk patterns across employment type, loan purpose, 
education level and credit scores.

## 🎯 Key KPIs
| KPI | Value |
|---|---|
| 💰 Total Loans | 255,347 |
| ⚠️ Default Rate | 11.61% |
| 💵 Avg Loan Amount | 127.58K |
| 📊 Avg Credit Score | 574.26 |

## 📊 Dashboard Visuals (12 Total)
1. KPI Card — Total Loans
2. KPI Card — Default Rate
3. KPI Card — Avg Loan Amount
4. KPI Card — Avg Credit Score
5. Donut Chart — Default vs Non-Default
6. Bar Chart — Loans by Loan Purpose
7. Bar Chart — Loans by Employment Type
8. Bar Chart — Loans by Education Level
9. Column Chart — Default Rate by Loan Purpose
10. Column Chart — Avg Credit Score by Employment
11. Column Chart — Avg Loan Amount by Loan Purpose
12. Slicer — Filter by Employment Type

## 💡 Key Insights
- **11.61%** default rate across 255,347 loans
- Average credit score of **574** is below healthy range
- Unemployed customers show highest default tendency
- Business loans carry highest average loan amounts

## 🔧 DAX Measures
- Total Loans = COUNTROWS('loan_default')
- Default Rate = DIVIDE(SUM([Default]),[Total Loans]) * 100
- Avg Loan Amount = AVERAGE('loan_default'[LoanAmount])
- Avg Credit Score = AVERAGE('loan_default'[CreditScore])

## 🚀 How To Open
1. Download [Power BI Desktop](https://powerbi.microsoft.com/desktop/) free
2. Download this repo
3. Open `Bank_Loan_Default_Dashboard_Vijayhgv.pbix`

## 🔧 KNIME Workflow
Automated ETL pipeline built using **KNIME Analytics Platform 5**
- ✅ 255,347 rows processed end-to-end
- ✅ Missing value imputation using Column Mean
- ✅ 128,653 defaulted loans isolated (50.4% default rate)
- ✅ KPIs summarized by Education level
- ✅ Clean output exported as CSV

## 👨‍💻 About Me
**Vijayhgv** — Aspiring Data Analyst from Anantapur, Andhra Pradesh
🔗 [Portfolio](https://vijayhgv.github.io) | [GitHub](https://github.com/vijayhgv)
