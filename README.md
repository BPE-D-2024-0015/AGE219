# Livestock and Crop Trend in Argentina

**Author:** DAUD MWANGALIKA  
**Registration Number:** BPE-D-2024-0015  
**Course Number:** AGE 219: Basics of Computer Programming  
**Course Instructor:** Dr. Kadeghe Fue, PhD, P.Eng (T)  

---

## 1. Problem Statement
Argentina stands out as an international hub for agronomic exports and agro-industrial activities. However, navigating structural performance shifts caused by changing agronomic conditions requires modern data-driven parsing tools. This agricultural engineering analysis addresses the challenge of identifying long-term historical crop yield trajectories and yield efficiency transformations across primary Argentine commodities. By tracking indicators over time, this project converts raw production metrics into actionable engineering data points to optimize farm inputs and resource allocation.

## 2. Data Source
The analytical repository evaluates data extracted from the Food and Agriculture Organization's statistical database (FAOSTAT). The core dataset consists of 10 individual data partitions tracking Argentine output parameters, including:
* `FAOSTAT_data_en_7-1-2026 (2).csv`
* `FAOSTAT_data_en_7-1-2026 (3).csv`
* `FAOSTAT_data_en_7-1-2026 (4).csv`
* `FAOSTAT_data_en_7-1-2026 (5).csv`
* `FAOSTAT_data_en_7-1-2026 (6).csv`
* `FAOSTAT_data_en_7-1-2026 (7).csv`
* `FAOSTAT_data_en_7-1-2026 (8).csv`
* `FAOSTAT_data_en_7-1-2026 (9).csv`
* `FAOSTAT_data_en_7-1-2026 (10).csv`
* `FAOSTAT_data_en_7-1-2026_supplementary.csv`

## 3. Methodology
The underlying parsing software leverages Python's scientific computing libraries to build an automated data engineering pipe:
* **Pandas:** Programmatically crawls, imports, and merges the 10 file inputs into a single global data frame, cleans out null entries, and filters records entirely focused on Argentina.
* **NumPy:** Processes swift vectorized conversions translating production metrics from kilograms per hectare ($kg/ha$) into standard metric tonnes per hectare ($t/ha$).
* **SciPy:** Evaluates mathematical trend changes over time using a linear data fit model (`scipy.stats.linregress`) to calculate correlation metrics.
* **Matplotlib:** Generates and exports clean plots according to engineering standards, incorporating descriptive titles, axis labels with metric parameters, legends, and readability grids.

## 4. Results & Conclusion
The automated data processing pipeline generated three primary figures outlining Argentina's production trends:

### 4.1 Production Intensity Over Time
The tracking visualization depicts the aggregated average yield trajectory over the observed calendar years, showcasing structural variations in historical farm management.
![Trend Analysis](trend_analysis.png)

### 4.2 Cross-Commodity Yield Performance
The comparative distribution map shows distinct yield outputs between index cash crops such as Sorghum, Potatoes, Oranges, and Grapes.
![Categorical Comparison](categorical_comparison.png)

### 4.3 Correlation and Trajectory Fit
The SciPy linear regression output shows the overall trend trajectory line plotted directly over yearly production data points.
![Correlation Fit](correlation_plot.png)

---

## Submission Registry
To submit this project for formal academic grading, the course instructor is tagged below:  
**Attention:** @kadefue
