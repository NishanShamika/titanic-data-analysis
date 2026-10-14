# Titanic Survival Analysis
 
Exploratory data analysis of the Kaggle Titanic dataset, using Python, pandas and matplotlib.
 
## Dataset
Kaggle: Titanic - Machine Learning from Disaster (train.csv, 891 passengers)
 
## What I did
1. Loaded and explored the data
2. Handled missing values:
   - Age (177 missing): filled with median
   - Embarked (2 missing): filled with mode
   - Cabin (687 missing): dropped, too many missing
3. Analysed survival rates with groupby
4. Created charts to visualise the results
 
## Key findings
- Overall survival rate was about 38.4%
- Women survived at 74.2%, men at only 18.9%
- 1st class survival was 63.0%, 2nd class 47.3%, 3rd class 24.2%
- Most passengers were aged 20-40
 
## Limitation
Filling missing ages with the median created an artificial
spike around age 28 in the age distribution.
 
## Tools
Python, pandas, matplotlib, Google Colab
 
## How to run
1. Download `train.csv` from the Kaggle Titanic competition page
2. Open the notebook in Google Colab
3. Upload `train.csv` to Colab (Files panel), or place it in Google Drive
4. Update the file path in the `pd.read_csv(...)` cell to match your location:
   - Colab upload: `pd.read_csv("train.csv")`
   - Google Drive: `pd.read_csv("/content/drive/MyDrive/<your-folder>/train.csv")`
5. Run all cells (Runtime → Run all)
