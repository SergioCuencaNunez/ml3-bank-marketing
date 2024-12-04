
# Unsupervised Learning on Bank Marketing Data

This project analyzes **bank marketing data** to uncover hidden patterns and customer behaviors using **unsupervised learning techniques**. It combines **Exploratory Data Analysis (EDA)**, **Principal Component Analysis (PCA)**, and **Clustering** to provide actionable insights for improving marketing campaigns.

## Objectives

1. **Pattern Discovery**: Uncover relationships between customer demographics, behavior, and campaign outcomes.
2. **Dimensionality Reduction**: Simplify complex data while retaining essential information.
3. **Customer Segmentation**: Group customers into meaningful clusters to enhance targeted marketing strategies.

## Methodologies and Insights

### 1. **Exploratory Data Analysis (EDA)**
   - **Key Findings**:
     - The majority of customers are aged 30-40 and hold university or high school degrees.
     - Personal loans are equally distributed, while house loans are prevalent among technicians, administrators, and blue-collar workers.
     - Campaign Effectiveness:
       - Pre-campaign: Optimum contact frequency was 3 calls.
       - During the campaign: If the second call fails, subsequent calls have diminishing returns.
       - Successful calls had longer durations.

### 2. **Principal Component Analysis (PCA)**
   - Reduced dimensionality using **Kaiser Rule**: 11 latent dimensions retained.
   - Variables with high variance:
     - `Age_group`, `job_retired`, `job_technician`, `job_blue-collar`, `education`, and `poutcome_success`.
   - **Encoding Methods**:
     - Ordinal, Binary, and Nominal encoding used for numeric transformation.
   - Observations:
     - Features were mostly orthogonal, ensuring minimal redundancy.

### 3. **Clustering Analysis**
   - Performed **K-Means Clustering**:
     - Optimal clusters: **11**, determined by the elbow method.
     - Silhouette Analysis:
       - High-quality clusters with proximity scores > 0.5.
       - **Cluster 7**: Most favorable (highest silhouette score).
       - **Cluster 3**: Least favorable (negative skew and lowest silhouette score).
     - Cluster distribution revealed significant variations in group sizes and behaviors.

## Results

### Customer Clusters
| Cluster | Size  | Key Characteristics                     |
|---------|-------|-----------------------------------------|
| 0       | 1,260 | Moderate density, balanced demographics |
| 2       | 7,509 | Largest group, significant aggregation  |
| 3       | 3,961 | Negative skew, lowest silhouette score  |
| 7       | 1,183 | Most favorable cluster                  |

### Key Outcomes
- **PCA**: Simplified visualization and analysis by reducing data complexity.
- **Clustering**: Enabled segmentation of the customer base into actionable groups for targeted marketing.

## Tools and Technologies

- **Languages**: Python
- **Libraries**: pandas, NumPy, scikit-learn, matplotlib, seaborn
- **Algorithms**: PCA, K-Means Clustering
- **Data Transformation**: Ordinal, Binary, and Nominal encoding

## Conclusion

Unsupervised learning methods such as PCA and clustering effectively provided insights into customer behavior and campaign optimization. By tailoring strategies for specific clusters, the bank can enhance its marketing success and improve customer engagement.

For further details or contributions, please contact **Elena Conderana** or **Sergio Cuenca**.
