# Social Media User Analysis: Clustering and Regression

## 📊 Project Overview
This project analyzes a social media user dataset to uncover patterns in user behavior, demographics, and income. Using **clustering techniques** and **linear regression**, the study explores relationships between age, time spent on platforms, and income, and identifies natural groupings within the data.

---

## 📁 Dataset Description
The dataset contains **1,000 entries** with the following key columns:

| Column | Description |
|--------|-------------|
| age | Age of the user |
| gender | Gender (male, female, non-living) |
| time_spent | Time spent on social media (in arbitrary units) |
| platform | Primary social media platform used |
| interests | Category of interest (Sports, Travel, Lifestyle) |
| location | Country of residence |
| demographics | Urban/Rural classification |
| occupation | Job category |
| income | Annual income |
| index | Unique identifier |
| information | Boolean flag for information availability |
| Out | Boolean flag for outlier |

### Descriptive Statistics:
- **Average age**: 41 years
- **Average time spent**: 5.03 units
- **Average income**: ~15,015 units
- **Age standard deviation**: 13.5 years
- **Income standard deviation**: 2,959 units

---

## 📈 Data Visualization

### 1. **Line Graph**
- **X-axis**: Age (20–60)
- **Y-axis**: Time spent (3.5–6.0)
- **Insight**: Users over 45 spend significantly less time on social media.

### 2. **Histograms**
- Age distribution (0–70 years)
- Time spent distribution (0–10 units)
- Income distribution (10,000–20,000 units)

### 3. **Heatmap (Correlation Matrix)**
- Variables: Age, Time spent, Income
- Diagonal values: 1.00 (perfect correlation with itself)
- Off-diagonal values: Near 0, indicating **weak linear relationships**

### 4. **Box Plot**
- Shows income distribution by age group
- Variation in whisker lengths and box sizes suggests income variability changes with age

---

## 🧠 Clustering Analysis

### Principal Component Analysis (PCA)
- Data reduced to two principal components for visualization
- **PCA Component 1** and **PCA Component 2** used as axes
- Five initial centroids used for clustering

### Elbow Method
- Tested **k = 2 to 10 clusters**
- Optimal **k** identified at the “elbow” where distortion reduction slows
- Helps balance cluster count and within-cluster variance

### Silhouette Analysis
- **Silhouette score** peaks at **k = 4 clusters**
- Indicates best cohesion and separation at 4 clusters
- Scores decline slightly beyond 4 clusters

### Clustering Results
- Data grouped into **4 distinct clusters** based on user behavior and demographics
- Clusters reflect patterns in platform usage, interests, and time spent

---

## 📉 Regression Analysis

### Linear Fitting
- **X-axis**: Time spent  
- **Y-axis**: Income
- **Fitted line**: Blue trend line showing positive relationship
- **Observation**: Income generally increases with time spent on social media

---

## 🛠 Tools & Techniques

### Libraries Used:
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- PCA for dimensionality reduction
- K-Means clustering with Elbow and Silhouette methods
- Linear regression for fitting

### Steps:
1. **Data preprocessing**: Cleaning, normalization, and encoding
2. **Exploratory Data Analysis (EDA)**: Visualizations and correlation analysis
3. **Clustering**: PCA, K-Means, and cluster evaluation
4. **Regression**: Fitting and interpretation

---

## 📌 Key Findings

1. **Age vs. Usage**: Older users (45+) spend less time on social media.
2. **Income Distribution**: Income varies across age groups, with highest average income at age 18.
3. **Weak Correlations**: Age, time spent, and income show minimal linear relationships.
4. **Optimal Clusters**: 4 clusters best represent the data structure.
5. **Income Trend**: Positive trend between time spent and income.

---

## 🚀 Future Work

- Explore **non-linear regression** models for better fitting
- Apply **advanced clustering algorithms** (e.g., DBSCAN, Gaussian Mixture Models)
- Incorporate **more features** like platform type and interests into regression
- Perform **time-series analysis** if longitudinal data is available

---

## 📚 References

- Scikit-learn Documentation
- VanderPlas, J. (2016). *Python Data Science Handbook*
- James, G., et al. (2013). *An Introduction to Statistical Learning*

---

## 👨‍💻 Author

**Ajay Santhosh Kavitha Veeramani**  
 


---

*This project is part of an Advanced Data Science (ADS) course focusing on clustering and regression techniques.*
