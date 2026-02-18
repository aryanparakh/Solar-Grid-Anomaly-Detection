# Solar-Grid-Anomaly-Detection
Unsupervised ML project to detect anomalies in Photovoltaic Power Grids

# **Temporal Pattern Discovery and Unsupervised Anomaly Detection in Photovoltaic Power Grids**

---

## **1\. Project Overview**

This project addresses the lack of labeled failure data in large-scale solar power plants. By applying **Advanced Unsupervised Machine Learning** and **Time Series Analysis**, we uncover hidden temporal structures in photovoltaic generation data to distinguish between environmental variability and genuine technical faults. The focus is on **Insight Generation** to support data-driven maintenance strategies.

---

## **2\. Folder Structure**



Plaintext  

│  
├── data/                                      \# Storage for raw datasets  
│   ├── Plant\_1\_Generation\_Data.csv            \# Power and yield metrics \[cite: 132\]  
│   └── Plant\_1\_Weather\_Sensor\_Data.csv        \# Environmental correlations \[cite: 133\]  
│  
├── Notebooks/                                 \# Documentation of core ML logic  
│   └── Temporal\_Tensors\_AML\_Analysis.ipynb    \# Clean, well-documented code \[cite: 84, 85\]  
│  
├── Reports/                                   \# Formal project documentation  
│   └── AIML\_Final\_Project\_Report.pdf          \# Detailed 10-page report \[cite: 74\]  
│  
└── README.md                                  \# Project execution guide \[cite: 87\]

---

## **3\. Dependencies**

To run this project locally or in Colab, the following Python libraries are required:

* **Data Handling:** `pandas`, `numpy`  
* **ML Algorithms:** `scikit-learn` (Isolation Forest, K-Means++)  
* **Time Series:** `statsmodels` (Additive Decomposition)  
* **Visualization:** `matplotlib`, `seaborn`

---

4\. How to Run the Project

1. **Environment Setup:** Install the necessary libraries using `pip install pandas numpy matplotlib seaborn statsmodels scikit-learn`.  
2. **Data Access:** Ensure the dataset files are correctly placed in the `data/` folder. Note: A Google Drive link is provided inside the notebook for direct access to large datasets.  
3. **Execute Analysis:** Open the Jupyter Notebook in the `Notebooks/` directory.  
4. **Sequential Execution:** Run the cells in order to perform:  
   * **Preprocessing:** Merging generation and weather metrics.  
   * **Time Series Decomposition:** Isolating Trend and Seasonality.  
   * **Anomaly Detection:** Identifying technical faults using Isolation Forest.  
   * **Asset Clustering:** Profiling inverter behavior with K-Means++.

---

5\. Summary of Core Insights

* **Efficiency Decay Tracking:** Detection of long-term downward trends signaling potential soiling (dust) on panels.  
* **Thermal Stress Window:** Identification of peak anomaly periods between 12 PM \- 2 PM, indicating overheating risks.  
* **Inverter Ranking:** Categorization of the 22 inverters into behavioral clusters to prioritize maintenance for underperforming units
