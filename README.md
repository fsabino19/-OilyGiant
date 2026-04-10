# TripleTen Sprint 9 Project – Machine Learning in Business: Oil Well Profitability Analysis

This is one of the applied machine learning projects I completed in the TripleTen Data Science program. It focused on using regression modeling and statistical analysis to help an energy company make a high‑stakes business decision about where to develop its next oil well.

---

# OilyGiant Region Profitability Prediction

OilyGiant Mining Company wants to identify the most profitable region for developing a new oil well. The company provided geological data from three different regions and asked for a data‑driven recommendation on where to invest.

The goal of this project was to build **regression models** to predict the volume of oil in new wells, estimate potential profit, and evaluate financial risk using statistical techniques.

---

# The Data

The dataset contains geological characteristics of oil wells across three regions. Each row represents one potential well site, along with the actual amount of recoverable oil.

The data was provided by TripleTen.

### Columns

- **id** — unique well identifier  
- **f0**, **f1**, **f2** — geological feature values (rock properties, depth measurements, etc.)  
- **product** — actual volume of recoverable oil (target variable)

Each region has its own dataset with the same structure.

---

# The Process

### 1. Data Preparation
- Loaded and explored datasets for all three regions.  
- Checked for missing values and validated feature distributions.  
- Confirmed that each region had different geological patterns, requiring separate models.

### 2. Train/Validation/Test Split
- Split each region’s dataset into training and validation sets.  
- Ensured consistent methodology across all three regions.

### 3. Model Training
Trained a **Linear Regression** model for each region to predict the volume of recoverable oil.

- Evaluated model performance using RMSE.  
- Compared prediction quality across regions.

### 4. Profit Calculation
- Calculated potential profit per well using provided business parameters.  
- Estimated total profit for each region based on selecting the top 200 predicted wells.

### 5. Risk Assessment
Used **bootstrapping** to:
- Estimate confidence intervals for regional profit.  
- Calculate the probability of financial loss.  
- Compare risk‑adjusted profitability across regions.

### 6. Decision Criteria
A region was considered viable if:
- Expected profit was high enough.  
- Risk of loss was below the company’s acceptable threshold.

---

# Results

The analysis identified one region as the most promising based on:
- Strong predicted profit  
- Low risk of financial loss  
- Stable model performance  

This project strengthened my understanding of:
- Regression modeling for real‑world business decisions  
- Bootstrapping and statistical confidence intervals  
- Evaluating financial risk using machine learning predictions  
- Comparing model performance across multiple datasets  
- Communicating results clearly to support strategic decisions  

Please refer to the Jupyter Notebook in this repository for the full workflow, code, and analysis.
