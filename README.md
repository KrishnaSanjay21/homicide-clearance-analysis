# Homicide-clearance-analysis
# 🔍 Analyzing Shifts in US Homicide Clearance Rates (1976–2023)

## 📌 Project Overview
Over the past half-century, the United States homicide clearance rate has dropped from roughly 74% to near 60%. This project utilizes 47 years of case-level data from the FBI's Supplementary Homicide Report (SHR) to quantitatively isolate the statistical drivers of this decline. 

Through extensive feature engineering and machine learning, this analysis proves that the drop in case resolutions is intrinsically linked to a sociological shift in the nature of crimes—specifically, the systemic rise of the "Anonymous" homicide.

## 🛠️ Tech Stack & Tools
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (Polynomial Regression, Random Forest, SVR)
* **Data Visualization:** Plotly, Power BI
* **Reporting:** LaTeX

## 📊 Key Findings
* **The Anonymity Gap:** Engineered an `Anonymous` feature (aggregating Stranger/Unknown relationships), which revealed a severe negative correlation (**r = -0.73**) with national clearance rates.
* **The Extrapolation Trap:** Demonstrated that while tree-based models (Random Forest) achieved exceptional historical accuracy ($R^2 = 0.976$), they mathematically failed at future time-series extrapolation.
* **Predictive Forecasting:** Validated a Polynomial Regression (Degree 3) model that successfully captured the non-linear asymptote of the data (**$R^2 = 0.81$, MAE = 1.32%**), forecasting a continued plateau unless modern data-centric investigative strategies (like IGG) are adopted.

## 📁 Repository Structure
* `notebooks/`: Contains the exploratory data analysis and machine learning pipeline.
* `report/`: Contains the formal LaTeX whitepaper detailing the methodology and strategic recommendations. 
* `visualizations/`: Correlation matrices and Plotly forecasting charts.

## 🔗 Full Report
[Click here to read the full formal PDF report.](https://github.com/KrishnaSanjay21/homicide-clearance-analysis/blob/main/Homicide_Clearance_Rates_Report_Vaddi.pdf)
