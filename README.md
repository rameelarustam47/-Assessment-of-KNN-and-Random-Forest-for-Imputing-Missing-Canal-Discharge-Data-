# -Assessment-of-KNN-and-Random-Forest-for-Imputing-Missing-Canal-Discharge-Data-
**Introduction**

Missing discharge data affects canal analysis and water management. Machine learning (ML) methods previously worked well for the QB (QR) Link Canal. This study applies the same methods to the MR Link Canal to test their performance under different data conditions.

**Methodology**

MR Link Canal data was preprocessed by converting dates, handling missing values, and applying Min–Max scaling. Three imputation methods were used:

Time-based interpolation (reference)

KNN imputation

Random Forest imputation

Results from ML methods were compared with interpolation using R², RMSE, MAE, MAPE, and Pearson correlation.

**Results**

Head discharge: Random Forest performed well and captured the overall trend, while KNN performed poorly.

Tail discharge: Both KNN and Random Forest showed weak performance with high errors and negative R² values.

Scaling improved numerical stability but did not significantly change performance.

**Interpretation**
ML methods worked well for the QB Link Canal because the data was smooth and stable. In contrast, MR Link Canal discharge is highly variable and strongly affected by operational controls, especially at the tail. KNN fails due to lack of similar patterns, and Random Forest cannot fully capture time-dependent behavior. Interpolation performs better because it follows the natural time structure of the data.



Machine learning–based imputation is not suitable for all canal systems. For MR Link Canal, time-based interpolation is more reliable than KNN and Random Forest. The study highlights the importance of understanding data behavior before applying ML methods.
