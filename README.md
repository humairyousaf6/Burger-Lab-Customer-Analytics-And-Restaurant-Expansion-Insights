# 🍔 Burger Lab Customer Analytics & Restaurant Expansion Insights

A data analytics project built with **Python, PySpark, Pandas, Matplotlib, and Seaborn** to analyze customer demographics, annual income, and restaurant spending patterns for Burger Lab.

The goal is to explore customer behavior and generate data-driven insights that can support decisions about opening a new restaurant branch in a potential location.

The project uses customer data to examine age distributions, gender composition, income patterns, restaurant spending, correlations between variables, and the relationship between customer age and spending.

---

## ✨ Features

- 📊 Customer demographic analysis
- 👥 Customer distribution by gender
- 🎂 Age group analysis
- 💰 Annual income analysis
- 🍔 Restaurant spending analysis
- 🔗 Correlation analysis between customer variables
- 📈 Histograms for customer distributions
- 🔍 Scatter plots for age versus restaurant spending
- 🧹 Missing-value inspection
- 🔢 Data type conversion and preprocessing
- ⚡ Large-scale data analysis using PySpark
- 📍 Data-driven insights to support restaurant expansion decisions

---

## 🎯 Business Problem

Burger Lab wants to evaluate a potential location for a new restaurant branch. The objective is to understand the characteristics and spending behavior of customers in the available dataset.

The analysis aims to answer questions such as:

- Which age groups are most represented among customers?
- How is the customer population distributed by gender?
- What are the annual income patterns of customers?
- How much do customers spend at the restaurant?
- Is there a relationship between age, income, and spending?
- Which customer segments may be valuable when evaluating a new branch location?

---

## 📊 Dataset

The project uses a customer dataset supplied for the analysis.

The notebook works with the following fields:

| Column | Description |
|---|---|
| `CustomerID` | Unique customer identifier |
| `Genre` | Gender category encoded numerically |
| `Age` | Customer age |
| `Annual_Income` | Customer annual income |
| `Resturant_Spending` | Restaurant spending measure |

The notebook also documents the original dataset using fields related to annual income and annual hotel/food spending.

---

## 🔬 Methodology

### 1. Data Loading

Load the customer dataset into a PySpark DataFrame and inspect the first records and schema.

### 2. Data Cleaning and Preprocessing

- Check for missing and null values.
- Inspect column data types.
- Convert customer attributes into numeric formats where required.
- Prepare the data for aggregation and visualization.

### 3. Exploratory Data Analysis

Explore the distributions of age, gender, income, and restaurant spending.

### 4. Data Aggregation

Use PySpark grouping and aggregation functions to examine customer counts and calculate minimum, maximum, and total annual income across age groups.

### 5. Correlation Analysis

Investigate relationships between:

- Age and gender
- Age and annual income
- Annual income and restaurant spending

### 6. Data Visualization

Create histograms and scatter plots using Matplotlib and Seaborn to identify customer distribution patterns and potential relationships.

---

## 📈 Key Findings

The notebook reports the following observations:

- **Age distribution:** The notebook identifies the 40–50 age range as having the highest customer representation.
- **Gender distribution:** The notebook reports 112 female customers and 88 male customers, using `0` for female and `1` for male.
- **Restaurant spending:** The notebook reports that many customers fall within a spending range of approximately 40,000–60,000.
- **Age and spending:** The notebook's interpretation suggests that younger customers visit more frequently or are more represented in the spending data.

These findings are the notebook's reported interpretations and should be validated against the dataset and plots before making business decisions.

---

## 🛠️ Tech Stack

### Data Processing
- Python
- PySpark
- Apache Spark
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn

### Development Environment
- Jupyter Notebook

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/humairyousaf6/Burger-Lab-Customer-Analytics.git
cd Burger-Lab-Customer-Analytics
```

### 2. Install Dependencies

```bash
pip install pyspark findspark pandas numpy matplotlib seaborn jupyter
```

### 3. Prepare the Dataset

Place the customer CSV file in your project directory and update the file path in the notebook.

For example:

```python
df = spark.read.csv(
    "Customer.csv",
    header=True,
    inferSchema=True
)
```

### 4. Run the Notebook

```bash
jupyter notebook
```

Open `BURGER_LAB_Analysis.ipynb` and execute the cells sequentially.

---

## 📁 Project Structure

```text
Burger-Lab-Customer-Analytics/
│
├── BURGER_LAB_Analysis.ipynb
├── Customer.csv
├── README.md
└── requirements.txt
```

The dataset filename and folder structure can be adjusted to match the files you upload. Do not upload private or confidential customer information to a public repository.

---

## 💡 Business Value

This project demonstrates how customer analytics can support restaurant planning by identifying demographic patterns, spending distributions, and potential customer segments.

The analysis can serve as an initial input for branch-location evaluation. A reliable expansion decision would also require location-specific information, such as population density, competition, rent, foot traffic, and local purchasing power.

---

## ⚠️ Limitations

- The analysis is based on the customer dataset provided.
- The notebook's observations do not establish causation.
- The dataset alone cannot confirm that a particular city or location will be profitable.
- The notebook uses a local Windows file path that must be updated for other environments.
- Some original column names and type-conversion steps may require adjustment to match the actual CSV schema.

---

## 👨‍💻 Author

**Muhammad Humair**

AI/ML & Automation Engineer

- Python
- Data Analytics
- PySpark
- Apache Spark
- Exploratory Data Analysis
- Data Visualization
- Machine Learning
