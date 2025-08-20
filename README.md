# Google Play Store Dataset - EDA & Feature Engineering

This project focuses on performing **Exploratory Data Analysis (EDA)** and **feature engineering** on the Google Play Store dataset to uncover insights about app popularity, installs, pricing trends, and more.

---

## Objective

With over 2.5 million apps available on the Google Play Store, understanding what makes an app successful is key for developers and businesses. This project aims to:

- Identify the most popular app categories
- Find the app with the largest number of installs
- Determine the largest app by size
- Analyze relationships between price, rating, installs, etc.

---

## Dataset

- **Source:** https://raw.githubusercontent.com/krishnaik06/playstore-Dataset/main/googleplaystore.csv 
- **Rows:** 10,841  
- **Columns:** 20  

---

## Project Steps

1. **Data Collection**
   - Loaded dataset from a public GitHub source
2. **Data Cleaning**
   - Removed invalid ratings (>5)
   - Converted `Reviews`, `Price`, `Installs`, and `Size` to appropriate datatypes
   - Handled missing values and outliers
3. **Feature Engineering**
   - Extracted Day, Month, and Year from `Last Updated`
4. **EDA**
   - Visualized top categories, price distribution, rating trends
   - Pie chart of app categories
   - Scatter plot of Price vs. Rating

---

## Visualizations

- Top 10 App Categories (Bar Plot)
- App Category Distribution (Pie Chart)
- Rating Distribution (Histogram)
- Price vs. Rating (Scatter Plot)

---

## Files Included

| File | Description |
|------|-------------|
| `GooglePlayStoreEDA.ipynb` | Jupyter Notebook with all analysis |
| `google_cleaned.csv` | Cleaned version of the dataset |
| `requirements.txt` | Python libraries used |

---

## ▶Usage

```bash
# Clone the repo
git clone https://github.com/<your-username>/google-playstore-eda.git
cd google-playstore-eda

# (Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook GooglePlayStoreEDA.ipynb

