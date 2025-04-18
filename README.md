# Clustering Analysis with Wine Dataset

This repo compares KMeans, Hierarchical Clustering, and MeanShift on the Wine dataset using six preprocessing techniques.

## Preprocessing Techniques
1. No Processing  
2. Normalized  
3. Transformed  
4. PCA  
5. T+N (Transformed + Normalized)  
6. T+N+PCA  

## Results

### KMeans Clustering

#### Silhouette Score  
![KMeans Silhouette](path/to/kmeans_silhouette.png)

#### Calinski–Harabasz Score  
![KMeans Calinski-Harabasz](path/to/kmeans_calinski.png)

#### Davies–Bouldin Score  
![KMeans Davies-Bouldin](path/to/kmeans_davies.png)

**Observation:** Best separation and compactness with PCA or T+N+PCA.

---

### Hierarchical Clustering

#### Silhouette Score  
![Hierarchical Silhouette](path/to/hierarchical_silhouette.png)

#### Calinski–Harabasz Score  
![Hierarchical Calinski-Harabasz](path/to/hierarchical_calinski.png)

#### Davies–Bouldin Score  
![Hierarchical Davies-Bouldin](path/to/hierarchical_davies.png)

**Observation:** Stable overall but higher Davies–Bouldin with raw/transformed data.

---

### MeanShift Clustering

#### Silhouette Score  
![MeanShift Silhouette](path/to/meanshift_silhouette.png)

#### Calinski–Harabasz Score  
![MeanShift Calinski-Harabasz](path/to/meanshift_calinski.png)

#### Davies–Bouldin Score  
![MeanShift Davies-Bouldin](path/to/meanshift_davies.png)

**Observation:** Consistent across preprocessings; benefits from normalization and PCA.

---

## Conclusion

- **Best Preprocessing:** T+N+PCA  
- **Top Algorithm:** KMeans with PCA or T+N+PCA  
- **Runner-up:** MeanShift when you don’t want to fix cluster count  

## How to Run

```bash
git clone https://github.com/your-username/your-repo.git
