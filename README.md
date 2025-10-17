# Mall Customer Clustering

This project performs customer segmentation using unsupervised learning techniques (K-Means and DBSCAN) on mall customer data. The goal is to identify groups of customers based on their annual income and spending score, helping businesses better understand customer behavior.

---

## Objective
Compare K-Means and DBSCAN clustering performance using the Silhouette Score to determine which method produces more meaningful customer segments.

---

## Project Structure
```
|- src/
   |- mall_customer_clustering.ipynb
|- .gitignore
|- README.md
|- requirements.txt
```

---

## Methodology
- **Dataset:** Mall Customers (via KaggleHub)  
- **Preprocessing:** Feature scaling with `StandardScaler`  
- **Outlier Removal:** IQR method  
- **K-Means:** Optimal `k` determined using the Elbow Method  
- **DBSCAN:** `eps` parameter tuned for maximum valid clusters  
- **Evaluation:** Silhouette Score comparison between both models  

---

## Results
- **K-Means Silhouette Score:** ~0.44  
- **DBSCAN Silhouette Score:** ~0.58  

DBSCAN produced slightly better clustering performance, though with more noise points (marked in red on plots).

---

## How to Run
1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd <repo-name>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:
   ```bash
   jupyter notebook src/mall_customer_clustering.ipynb
   ```

---

## Author
**Tasneem Helal**  
Mechatronics Engineer
