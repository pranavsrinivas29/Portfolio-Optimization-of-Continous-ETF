 Machine Learning for Dynamic Portfolio Management
==========================


### Background and Overview

A portfolio denotes a collection of investments owned by an individual, corporation, or financial entity. These
types of investments may include various asset types, such as equities, fixed income securities, commodities,
and real estate. Portfolio optimization seeks to maximize the expected return for a tolerable level of risk.
This problem lies at the heart of quantitative finance, where mathematical models guide investment decisions
rather than intuition or historical bias. Portfolio optimization is a practical necessity for asset managers,
institutional investors, and algorithmic trading systems. It plays a central role in wealth management,
pension fund allocation, hedge fund strategies, and Exchange-Traded Fund (ETF) management.

This study aims to extend the previously outlined methodologies while directly addressing the associated
practical limitations, thereby enhancing both the rigor and relevance of the proposed approaches. First,
it evaluates model performance across multiple investment horizons, that is, weekly (short-term), monthly
(medium-term), and annual (long-term), to uncover horizon-sensitive patterns in portfolio performance.
Second, it compares temporal (LSTM) and non-temporal (OLS, LASSO, RF, Boosted Trees (BT)) models
within a shared data environment and rolling-window setup, allowing for consistent performance bench-
marking. Third, it deviates from rule-based portfolio construction by employing weight-based optimization
for the objective function of the composite scores, which is formulated by inculcating different risk measures
to dynamically allocate capital.

Finally, this study explicitly incorporates turnover penalties and transaction-cost drag, resulting in a
practical, cost-aware, and risk-adjusted portfolio framework to replicate real-world deployment. By address-
ing these interlinked dimensions and model type, allocation flexibility, risk measurement, and rebalancing
cost, this research offers a more comprehensive solution to data-driven portfolio optimization.

 PROJECT STRUCTURE NOTES
==========================

Name: Pranav Srinivas Venkatesh
Matriculation Number: 1678255
Master Thesis: Machine Learning for Dynamic Portfolio Optimization

Report Folder:
-------------
This folder contains detailed thesis report which was submitted.

Data Folder:
-------------
- Contains all locally saved data files.
- These data files are loaded from external sources and stored for further processing or modeling.

Data Download and caching.ipynb:
----------------------------------
- This notebook contains the script for downloading data from an external API.
- The downloaded data is then saved into the 'Data' folder for local use.

Model_artifacts Folder:
-------------------------
- Stores all pre-trained machine learning models and scalers.
- These artifacts are used for inference or further evaluation without retraining the models.

Model_name_2022_final_code.ipynb:
-----------------------------------
- Contains the complete code for running forecasting tasks specifically for the year 2022.
- Includes data loading, preprocessing, model loading/training, prediction, and result saving and portfolio optimization steps.

Model_name_2024_final_code.ipynb:
-----------------------------------
- Contains the complete code for running forecasting tasks specifically for the year 2024.
- Includes data loading, preprocessing, model loading/training, prediction, and result saving and portfolio optimization steps.

Model-wise-scores.ipynb:
--------------------------
- Contains ETF-wise scores for all forecasting models across all time horizons.

requirements.txt:
------------------
- Lists all required Python libraries along with their specific version numbers.
- Ensures environment consistency across different systems for reproducibility.
