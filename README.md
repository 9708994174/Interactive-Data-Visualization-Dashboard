# 🚗 Interactive Data Visualization Dashboard using R

This project is an interactive data dashboard built using **R**, **Flexdashboard**, and various visualization libraries. It presents analytical insights from car failure data across U.S. states, focusing on key metrics such as labor costs, failure mileage, and failure frequency.

---

## 📌 Project Overview

- **Title**: RK's Dashboard
- **Technology**: R, RMarkdown, Flexdashboard
- **Focus**: Visual analysis of car failures in the United States
- **Data Source**: Local dataset (`carFailureData.csv`)
- **Key Dimensions**: State, Failure Month (`fm`), Labor Cost (`lc`), Mileage

---

## 💡 Features

- 🔍 **Summary Statistics** via value boxes (e.g., avg. mileage, labor cost)
- 📊 **Charts**:
  - Bar chart of failures by state
  - Pie chart of top failure states
  - Bar chart and scatter plot for `fm` vs. `Mileage`
  - Box plots for labor cost across states
- 🗺️ **Interactive Map** using Highcharter
- 📈 **Pivot Table** using `rpivotTable`
- 📋 **Data Table** with filtering and pagination
- 📅 Automatically generated report date

---

## 📁 File Structure

```bash
Interactive-Data-Visualization-Dashboard/
├── dashboard.Rmd                  # Main dashboard source file
├── data/
│   └── carFailureData.csv         # Car failure dataset
├── www/
│   └── custom.css                 # (Optional) Custom styles
├── images/
│   └── dashboard_preview.png      # Dashboard screenshot
└── README.md                      # Project documentation
````

---

## 📦 Libraries Used

```r
library(flexdashboard)
library(knitr)
library(DT)
library(rpivotTable)
library(ggplot2)
library(plotly)
library(dplyr)
library(openintro)
library(highcharter)
library(ggvis)
```

---

## 🛠️ How to Run the Dashboard

1. Clone this repo or download the files.

2. Open `dashboard.Rmd` in **RStudio**.

3. Install any missing libraries with:

   ```r
   install.packages(c("flexdashboard", "plotly", "DT", "rpivotTable", "highcharter", "ggvis", "openintro", "dplyr"))
   ```

4. Run the dashboard by clicking **"Run Document"** or rendering with:

   ```r
   rmarkdown::run("dashboard.Rmd")
   ```

📌 **Note**: Update the CSV path in the `read.csv()` function if necessary.

---

## 📷 Preview

<img width="1919" height="1051" alt="Screenshot 2025-04-26 092606" src="https://github.com/user-attachments/assets/b576af61-3f9f-47f6-94aa-ba38e3c1aeab" />


---

## 🧠 Insights Provided

* Which U.S. states report the highest vehicle failure rates
* Comparison of labor cost by state
* Visual relationship between failure month and mileage
* Heatmap of state-month combinations using a pivot table
* Average mileage and labor cost across all records

---

## 🧾 Example Summary Report (Auto-generated in dashboard)

> * Total Failures: 1700+
> * Avg. Labor Cost: \$160
> * Avg. Mileage at Failure: 58,000 miles
> * Max Failure Month: 12
> * Most Frequent States: CA, TX, FL, MA
> * Report generated on: July 13, 2025

---

## 🙋‍♂️ Author

**Rahul Kumar**
BTech Computer Science | Aspiring Data Scientist
📫 [LinkedIn](https://www.linkedin.com/in/rahulkr11) | 🌐 [GitHub](https://github.com/9708994174)

---

## 📄 License

This project is licensed under the **MIT License**. Feel free to use and modify it.

---

## 📌 Acknowledgements

* Dataset inspired by automotive maintenance analytics
* Visualization support by R open-source community
* Developed as part of an academic data visualization portfolio

```

