# Geographic Consumer Clustering using K-Means

## Project Overview

This project uses the K-Means Clustering algorithm to group real estate properties into different geographic consumer segments based on property location and customer characteristics. The project helps identify similar regions for market analysis and business expansion.

---

## Problem Statement

Real estate companies often need to identify different consumer regions based on property and customer data. Manual analysis is difficult when dealing with large datasets. This project automatically clusters properties into different geographic segments using Machine Learning.

---

## Objective

- Analyze real estate consumer data.
- Group similar properties using K-Means Clustering.
- Visualize consumer clusters on a geographic map.
- Support business decision-making through data segmentation.

---

## Dataset

The dataset contains the following features:

| Feature | Description |
|---------|-------------|
| PropertyID | Unique property ID |
| Latitude | Geographic latitude |
| Longitude | Geographic longitude |
| Price | Property price |
| Area_sqft | Property area in square feet |
| Bedrooms | Number of bedrooms |
| ConsumerIncome | Customer annual income |

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

---

## Machine Learning Algorithm

- K-Means Clustering

---

## Project Workflow

1. Import required libraries.
2. Load the dataset.
3. Select important features.
4. Standardize the data.
5. Find the optimal number of clusters using the Elbow Method.
6. Train the K-Means model.
7. Assign cluster labels.
8. Visualize geographic consumer clusters.
9. Save the clustered dataset.

---

## Project Structure

```
04_Geographic-Consumer-Clustering-KMeans
│
├── Dataset
│   └── real_estate_consumer_data.csv
│
├── Notebook
│   └── Geographic_Consumer_Clustering_KMeans.ipynb
│
├── Output
│   ├── clustered_real_estate_output.csv
│   ├── elbow_method.png
│   └── geographic_clusters.png
│
├── Model
│   ├── kmeans_model.pkl
│   └── scaler.pkl
│
├── Images
│   ├── elbow_method.png
│   └── geographic_clusters.png
│
├── README.md
│
└── requirements.txt
```

---

## Results

- Successfully grouped properties into different consumer clusters.
- Identified the optimal number of clusters using the Elbow Method.
- Generated geographic cluster visualization.
- Exported clustered dataset for further analysis.

---

## Future Enhancements

- Interactive geographic maps using Folium.
- Support larger real estate datasets.
- Automatic cluster prediction for new properties.
- Dashboard using Streamlit.

---

## Author

**Ashwin**

Machine Learning Enthusiast | Python | Data Science | Scikit-learn
