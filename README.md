NET ZERO SMART METERS 
=====================

What is this?
-------------
Data pipeline for Northern Powergrid (NPG) smart meter data. 


Folder Setup
------------
data/raw/       -> Drop the massive NPG csv here. (Ignored by git)
data/processed/ -> Cleaned, time-aligned data goes here.
notebooks/      -> Jupyter files (EDA, geographic mapping).
scripts/        -> Python ETL modules.
outputs/        -> Generated graphs and reports.

How to run it
-------------
1. Clone the repo and cd into it.
2. pip install -r requirements.txt
3. Download the NPG dataset and put the CSV in data/raw/
4. Run notebooks/01_data_loading_and_cleaning.ipynb

Notes & Project Status
----------------------
- The raw NPG CSVs are 700MB+. They are explicitly ignored in .gitignore. Do not try to commit them or GitHub will reject the push.
- WP1 (architecture & git setup) is complete. 
- WP2/3 (Time-series EDA) in progress.