## Exploratory Data Analysis – EV-SensorGuard

Exploratory Data Analysis was performed on three EV battery sensor features: internal resistance, peak temperature during fast charging, and average charging time.

### Key Findings

1. **Internal Resistance:** The distribution is positively skewed, with 5.88% of observations identified as statistical outliers using the IQR method.

2. **Charging Temperature:** The distribution is approximately bell-shaped, with 0.64% statistical outliers. Some negative temperature readings require further validation.

3. **Charging Time:** The distribution is strongly right-skewed, with 7.17% statistical outliers. Several unusually long charging durations were observed.

4. **Correlation Analysis:** All three sensor pairs exhibit weak linear correlations, indicating limited linear association between the selected features.

### Conclusion

The dataset contains unusual sensor readings and different distribution patterns across features. These findings support further investigation using unsupervised anomaly detection algorithms such as Isolation Forest and Local Outlier Factor (LOF).

Statistical outliers are retained for model development rather than removed, since detecting unusual sensor behaviour is the primary objective of this project.
