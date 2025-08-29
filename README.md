#  Mall Customer Segmentation Using K-Means Clustering

##  Overview
This project applies **K-Means clustering**, an unsupervised learning technique, on the **Mall Customers** dataset to uncover meaningful customer segments—based on features like age, annual income, and spending patterns.

---

##  Dataset Details
- **Source:** Kaggle — *Mall Customer Segmentation Data* :contentReference[oaicite:0]{index=0}  
- **Entries:** ~200 customers  
- **Features:**
  - `CustomerID`
  - `Gender`
  - `Age`
  - `Annual Income (k$)`
  - `Spending Score (1-100)`

---

##  Workflow Steps

1. **Exploratory Data Analysis (EDA):**  
   - Visualized distributions (age, income, spending score)  
   - Analysed gender breakdown  

2. **Cluster Analysis:**
   - Extracted the key features (income vs. spending score, optionally age in 3D)
   - Applied the **Elbow Method** to determine optimal cluster number (commonly K = 5)
   - Ran **K-Means** clustering
   - Visualized clusters in 2D scatter plots and optional 3D plots (age, income, spending)
   - Labeled each data point with its cluster ID

3. **Interpretation:**
   - Analyzed clusters—e.g., high income/high spending, low income/low spending, etc.
   - Examined cluster sizes and characteristics

---

##  How to Run
```bash
pip install -r requirements.txt
```
```bash
jupyter notebook mall-customer-segmentation.ipynb
```

##  Key Insights

- **Optimal clusters chosen:** 5 (as indicated by the Elbow Method)  
- **Clusters revealed distinct groups:**  
  - “High earners with high spending”  
  - “Low income / low spending” segments  
- **Age-based 3D visualization** further showed demographic overlaps across clusters  

---

##  Future Work

- Experiment with alternative clustering algorithms (e.g., DBSCAN, Hierarchical Clustering)  
- Evaluate clusters using metrics like Silhouette Score or Davies–Bouldin Index  
- Incorporate additional features (e.g., gender encoding, behavior-based metrics)  
- Build a simple interactive dashboard (using Streamlit or Flask) for visual exploration  

---

##  Author

Soumil Malik — An **AI/ML & MLOps enthusiast**, currently a **final-year student in India**, preparing for higher education exams and developing practical ML projects.

---

##  License

Open for **educational and research purposes**.  
Recommended: [MIT License](https://opensource.org/licenses/MIT)  

