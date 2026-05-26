For your GitHub repository, here are suggestions for a brief repository description and a structured README file based on the analysis of Treasury Bond yield changes found in the sources.

### **Repository Description**
**PCA-Treasury-Yield-Analysis**: A Python-based Principal Component Analysis (PCA) of daily yield changes for U.S. Treasury securities (1-month to 5-year maturities) using FRED data.

---

### **README.md Content**

# PCA Analysis of Treasury Bond Yield Changes

This project performs a **Principal Component Analysis (PCA)** on the daily percentage changes of U.S. Treasury Bond yields. The goal is to identify the underlying factors that drive yield movements across different maturities.

## **Overview**
The analysis explores the relationship between various Treasury maturities (1-Month, 6-Month, 1-Year, 3-Year, and 5-Year). By applying PCA, we reduce the dimensionality of the yield data to understand how much of the total variance is explained by the primary principal components (e.g., Level, Slope, and Curvature).

## **Key Features**
*   **Data Acquisition:** Automated data retrieval from the **FRED (Federal Reserve Economic Data)** API for the period of **October 11, 2024, to April 11, 2025**.
*   **Statistical Analysis:** 
    *   Calculation of Correlation and Covariance matrices.
    *   Data standardization to ensure all maturities are on the same scale.
*   **PCA Implementation:** 
    *   Eigenvalue and Eigenvector estimation.
    *   Calculation of Principal Component scores.
*   **Visualization:** 
    *   **Heatmaps** for visualizing correlations between daily yield changes.
    *   **Scree Plots** to determine the significance of each principal component.

## **Analysis Highlights**
Based on the provided dataset:
*   **PC1** explains approximately **65.39%** of the total variance.
*   **PC2** explains **21.04%**.
*   **PC3** explains **10.08%**.
*   Together, the first three components account for **96.51%** of the variability in Treasury yield changes.

## **Dependencies**
*   Python 3.x
*   Pandas
*   NumPy
*   Matplotlib
*   Seaborn
*   FredAPI

## **Data Source**
The yield data used in this project is sourced from the Federal Reserve Bank of St. Louis (FRED) using the following series IDs: `DGS1MO`, `DGS6MO`, `DGS1`, `DGS3`, and `DGS5`.

---

*Note: This analysis was conducted as part of a GWP (Group Weekly Project) focused on financial data modeling.*
