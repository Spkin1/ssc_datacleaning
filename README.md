# Data Preprocessing & Cleansing
An end-to-end, production-ready Python showcase notebook demonstrating advanced data engineering, feature engineering, and data cleansing techniques designed to transform raw, volatile datasets into high-fidelity inputs for machine learning.

##  Overview & Objectives
Real-world data is inherently messy, corrupted, and poorly formatted. This repository shows data preprocessing methodologies. It implements logic blocks to tackle real-world anomalies across diverse data streams—including numerical logs, structural metrics, geospatial configurations, time-series intervals, and natural language properties.

### Key Preprocessing Pillars Highlighted:
1. **Systematic Missingness Evaluation**: deletions to mathematically justify column/row drop thresholds versus sequential forward/backward padding.
2. **Feature Engineering via Scaling & Scaling Adjustments**: Implementing standard MinMaxScaler bounds alongside advanced **Box-Cox Power Transformations** to stabilize variance and normalize heavily skewed distributions into clean Gaussian bells.
3. **Advanced Datetime Feature Parsing**: Parsing heterogeneous string timestamps with varying structures into unified `datetime64[ns]` objects for time-series extraction.
4. **Character Encoding Conflict Resolution**: Building encoding diagnostics to handle text corruption (e.g., `Windows-1252` to standard `UTF-8` serialization) without losing payload semantics.
5. **Fuzzy String Matching & De-duplication**: Utilizing Levenshtein token distance models to fix inconsistent user entries, typos, and syntax scattering automatically.

---

##  Tech Stack & Dependencies
The notebook is built to comply with PEP 8 style standards and operates on production-grade scientific libraries:
* **Python 3.12+**
* **Core Analytics**: `pandas`, `numpy`
* **Statistical Modeling & Preprocessing**: `scipy.stats`, `mlxtend`
* **Text Cleansing & String Clustering**: `fuzzywuzzy` / `Levenshtein`, `charset_normalizer`
* **Data Visualization**: `matplotlib`, `seaborn`
---

##  Dataset Source
If the data is not available in Data_103 folder here, it is due to the lager size of the data and the data can be access from the official Kaggle Data Cleaning course website  
https://kaggle.com/learn/data-cleaning/data

---

## Quick Start & Evaluation
To explore the implementation and run the data cleaning pipelines locally, clone the repository and run the Jupyter interface:

```bash

# Install required dependencies
pip install pandas numpy scipy mlxtend fuzzywuzzy Levenshtein charset-normalizer seaborn matplotlib jupyter

# Boot up the notebook environment
jupyter notebook ssc_datacleaning.ipynb
```

---
