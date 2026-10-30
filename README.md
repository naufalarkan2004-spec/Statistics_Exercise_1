Statistics Analysis — Potret Kebahagiaan Indonesia

Descriptive statistics exercise on the World Happiness Report 2026, focused on one question: Are Indonesians getting happier? The repo contains the analysis notebook and the presentation built from it.

Author: Naufal Arkan Muhana

Contents
File	Description
NaufalArkanMuhana_DescStats_WHR_Template.ipynb	Analysis notebook (Python) with code, outputs and written interpretations
Potret Kebahagiaan Indonesia_ Are We Getting Happier_ ... (3).pdf	16-slide presentation of the findings (Bahasa Indonesia)
Dataset
Source: World Happiness Report 2026 (WHR26_Data_Figure_2.1.xlsx)
Size: 2,116 rows x 13 columns (country-year observations, 2011–2025)
Key variable: Life Ladder (life evaluation, 0–10 scale)
Explanatory variables: Log GDP per capita, Social support, Healthy life expectancy, Freedom to make life choices, Generosity, Perceptions of corruption
Scope of the analysis: Indonesia, 2021–2025 (5 years), compared with the global sample and ASEAN countries

The dataset file is not included in this repo. Download it from the link above and place it next to the notebook.

Notebook structure
Data preparation & exploration – load, inspect, missing values, filter Indonesia (df_idn), variable classification
Central tendency – mean, median, mode; Indonesia vs global average
Spread – range, variance, standard deviation, IQR, coefficient of variation; outlier detection (IQR and Z-score)
Distribution – histograms, skewness and kurtosis, KDE, Indonesia vs global distribution
Visualization & relationships – trend line chart, ASEAN comparison, correlation with explanatory factors
Key findings
Mean Life Ladder for Indonesia (2021–2025) is 5.464 (median 5.568, mode 5.617).
Variation is small: standard deviation 0.189, coefficient of variation 3.46%, and no outliers by IQR or Z-score.
Global rank stays around the 80s; the score has improved since 2023 after the post-pandemic dip.
Freedom to make life choices shows the strongest correlation with Life Ladder (r = 0.893, p = 0.042), followed by generosity (r = −0.878, p = 0.050) and social support (r = 0.787, p = 0.114). GDP, life expectancy and corruption are weak and non-significant.
Decomposing the 2021→2025 rise (+0.38), freedom (+0.42) and social support (+0.35) contribute most; generosity (−0.17) and the unexplained residual (−0.28) pull it down.
Indonesia ranks 5th of 7 ASEAN countries with 2021–2025 data (Vietnam and Laos have none), with Singapore consistently leading.

With only five yearly observations, correlations are indicative rather than conclusive.

Tech stack

Python, pandas, NumPy, SciPy, Matplotlib, Seaborn, Jupyter Notebook

How to run
bash
pip install pandas numpy scipy matplotlib seaborn openpyxl jupyter
jupyter notebook NaufalArkanMuhana_DescStats_WHR_Template.ipynb

Make sure WHR26_Data_Figure_2.1.xlsx is in the same folder as the notebook.

Source

World Happiness Report 2026.
