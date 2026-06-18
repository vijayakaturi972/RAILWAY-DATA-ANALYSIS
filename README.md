# 🚆 Indian Railway Data Analysis

> **Data Engineering Internship Project** — End-to-end data pipeline covering ingestion, cleaning, transformation, aggregation, and visualization of Indian Railway train schedule data.

---

## 📌 Project Overview

This project was completed as part of a **Data Engineering Internship**. The objective was to build a structured data analysis pipeline on a real-world Indian Railway dataset — covering all stages from raw data loading to deriving actionable insights through visualizations.

The project demonstrates core data engineering skills including:
- Data ingestion and inspection
- Data cleaning and standardization
- Filtering, grouping, and aggregation
- Feature engineering (day categorization)
- Pattern analysis and visualization

---

## 📂 Project Structure

```
Data_Engineering_Internship/
├── Railway_Analysis.ipynb      # Main Jupyter Notebook (all tasks)
├── Railway_info.csv            # Source dataset (Indian Railway schedule)
├── screenshots/                # Output visualizations
│   ├── 01_train_distribution_by_day.png
│   ├── 02_top_10_source_stations.png
│   ├── 03_weekday_vs_weekend.png
│   └── 04_dataset_preview.png
└── README.md
```

---

## 📊 Dataset Description

**File:** `Railway_info.csv`  
**Records:** 11,113 train entries  
**Source:** Indian Railway train schedule data

| Column | Description |
|---|---|
| `Train_No` | Unique train number |
| `Train_Name` | Name of the train |
| `Source_Station_Name` | Starting station of the train |
| `Destination_Station_Name` | Ending station of the train |
| `days` | Day(s) of the week the train operates |

**Key Facts:**
- 11,113 unique trains in the dataset
- 921 unique source stations across India
- Covers all 7 days of the week
- CST-MUMBAI is the busiest source station (513 trains)

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Python 3** | Core programming language |
| **Pandas** | Data loading, cleaning, transformation, aggregation |
| **Matplotlib** | Bar charts, line charts, data visualization |
| **Seaborn** | Heatmap and advanced visualizations |
| **Jupyter Notebook** | Interactive development environment |

---

## 📋 Tasks Completed

### Task 1 — Data Loading & Exploration
- **1.1** Loaded dataset using Pandas; inspected structure, shape, and data types
- **1.2** Computed basic statistics: total trains, unique source/destination stations, top stations by frequency
- **1.3** Checked for missing values; standardized station names to uppercase for consistency

### Task 2 — Filtering, Grouping & Enrichment
- **2.1** Filtered trains operating on Saturday; identified trains departing from CST-MUMBAI
- **2.2** Grouped by source station and by operating day; computed average trains per day
- **2.3** Engineered a new `Day_Category` feature classifying each train as **Weekday** or **Weekend**

### Task 3 — Pattern Analysis & Insights
- **3.1** Analyzed day-wise distribution of train operations
- **3.2** Calculated percentage breakdown of weekday vs. weekend trains; derived key dataset insights

### Task 4 — Data Visualization
- **4.1** Bar chart: Distribution of train operations by day of the week
- **4.2** Line chart: Trend of trains per operating day
- **4.3** Heatmap: Visual correlation across day-station patterns

---

## 💡 Key Insights

1. **11,113 trains** are recorded in the dataset across India
2. **CST-MUMBAI** is the busiest originating station with **513 trains**
3. **Friday** sees the highest number of train operations among weekdays
4. The majority of trains (~80%) operate on **weekdays**, while ~20% operate on **weekends**
5. **921 unique source stations** are covered, showing the vast reach of Indian Railways

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/railway-data-analysis.git
   cd railway-data-analysis/Data_Engineering_Internship
   ```

2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Railway_Analysis.ipynb
   ```

4. Run all cells from top to bottom.

---

## 🏆 Internship Completion

This project was completed as part of a **Data Engineering Internship**, demonstrating proficiency in:
- Real-world dataset handling with Python and Pandas
- Data cleaning and quality assurance
- Feature engineering and data transformation
- Exploratory Data Analysis (EDA)
- Data visualization and insight generation

---

## 📧 Contact

Feel free to connect on [LinkedIn](https://www.linkedin.com/) for any questions or collaboration.

---

*Made with ❤️ using Python & Pandas*
