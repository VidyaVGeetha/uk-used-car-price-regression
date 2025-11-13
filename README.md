# UK Used Car Price Prediction Using Regression Analysis

This project explores how different car features influence used car prices in the UK.  
Using a clean, synthetic dataset of UK used cars, the notebook walks through Exploratory Data Analysis (EDA) and regression plots to understand the impact of **mileage**, **manufacturing year**, and **engine size** on **price**.

The project is designed as a **portfolio piece** for an aspiring Data Analyst, with clear step-by-step code, comments, and visualisations.

---

## 🎯 Objectives

- Load and explore a UK used car dataset using **pandas**
- Perform basic EDA: missing values, duplicates, data types, and summary statistics
- Visualise relationships between:
  - **Mileage vs Price**
  - **Year vs Price**
  - **Engine Size vs Price**
- Create **regression plots** using `seaborn.regplot`
- Practise making plots more **attractive and readable** with custom styles, colours, and labels
- Interpret the trends in a way that is useful for business and pricing decisions

---

## 📂 Dataset

**File:** `UK_Used_Car_Prices.csv`

Each row represents one used car listing.

**Columns:**

- `Make` – Car manufacturer (e.g., Ford, BMW, Toyota)
- `Model` – Model label
- `Year` – Manufacturing year of the car
- `Mileage` – Distance driven (in km)
- `Engine_Size_L` – Engine size in litres
- `Fuel_Type` – Petrol, Diesel, Hybrid, Electric
- `Price` – Used car price in GBP (£)

The dataset is already clean, with no missing values or duplicate rows, which makes it ideal for practising EDA and regression visualisation.

---

## 🛠 Tech Stack

- **Language:** Python
- **Libraries:**
  - `pandas` – data loading and manipulation
  - `numpy` – numerical operations
  - `matplotlib` – plotting
  - `seaborn` – statistical visualisation (regression plots)

---

## 📊 Notebook Structure

All analysis is done in the Jupyter notebook:

`uk-used-car-price-prediction.ipynb`

The notebook is organised into clearly labelled steps:

### Step 1–3: Setup and Data Loading
- Install (if needed) and import required libraries
- Read `UK_Used_Car_Prices.csv` into a pandas DataFrame
- Preview the first few rows with `head()`

### Step 4: Exploratory Data Analysis (EDA Basics)
- **4.1:** Check for missing values in each column  
- **4.2:** View data types and structure with `info()`  
- **4.3:** Check for duplicate rows  
- **4.4:** Explore unique values in categorical columns (Make, Model, Fuel_Type)  
- **4.5:** Generate descriptive statistics for numerical features (Year, Mileage, Engine_Size_L, Price)

### Step 5: Mileage vs Price — Regression Plot
- Create a scatter plot of **Mileage vs Price**
- Add a regression line using `sns.regplot`
- Customise:
  - figure size
  - style (`sns.set_style`)
  - scatter point transparency, colour, and size with `scatter_kws`
  - regression line colour and thickness with `line_kws`
- Interpret the result: as mileage increases, used car price tends to decrease.

### Step 6: Year vs Price — Regression Plot
- Plot **Year vs Price** with a regression line
- Improve readability of the x-axis:
  - show **year values as integers** instead of floats (e.g. 2010, not 2010.0)
- Interpret the result: newer cars (higher year) tend to have higher prices.

### Step 7: Engine Size vs Price — Regression Plot
- Plot **Engine Size vs Price**
- Apply a different colour theme and style
- Interpret the trend: cars with larger engines are generally more expensive, but the relationship is weaker compared to Year vs Price.

Each main section also contains short comments explaining **what the code does** and **why it is relevant** for regression analysis.

---

## 📌 How to Run the Notebook

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/uk-used-car-price-regression.git
   cd uk-used-car-price-regression

________________________________
🔍 Key Insights

Mileage vs Price:
There is a clear negative relationship. Higher mileage cars tend to be cheaper, which matches real-world expectations for used cars.

Year vs Price:
There is a strong positive relationship. Newer cars are generally more expensive, and the regression line clearly slopes upwards.

Engine Size vs Price:
Larger engines are associated with slightly higher prices, but the relationship is weaker. Price is also affected by other factors such as year and mileage.

These plots show how visual regression can help explain pricing patterns to non-technical stakeholders.

__________________________________
💼 Why This Project Matters for a Data Analyst Role

This project demonstrates:

Ability to load and explore real-world style tabular data

Understanding of basic EDA techniques

Skill in building clear, interpretable visualisations

Use of regression plots to reveal relationships between features and a target variable

Clean, well-commented Jupyter notebook structure that others can follow
_______________________________________
## 👤 Author

**Vidya Vishnuvihar Geetha**  
Aspiring Data Analyst  
Focused on building real-world Python, EDA, and visualisation projects.  

📧 Email: [vidyavgk@gmail.com](mailto:vidyavgk@gmail.com)
