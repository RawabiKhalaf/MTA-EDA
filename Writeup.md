# NYC Self-Driving Taxis Distribution Plan
Rawabi Alharbi

## Abstract
The goal of this project was to ...      

## Design


## Data
The data used is the Metropolitan Transportation Authority (MTA) which contains 2474417 rows and 11 columns. The dataset is a series of data files containing numbers of cumulative entries and exits by stations, turnstile, along with their dates and time. The data records are weekly produced and mostly collected every 4 hours. The data obtained from http://web.mta.info/developers/turnstile.html and it includes 11 columns and the following is the description of each feature:

## Algorithms

*Feature Engineering*
1.
2.
3.
4.

*Models*
  
Logistic regression, k-nearest neighbors, and random forest classifiers were used before settling on random forest as the model with strongest cross-validation performance. Random forest feature importance ranking was used directly to guide the choice and order of variables to be included as the model underwent refinement.

*Model Evaluation and Selection*
  
The entire training dataset of 59,400 records was split into 80/20 train vs. holdout, and all scores reported below were calculated with 5-fold cross validation on the training portion only. Predictions on the 20% holdout were limited to the very end, so this split was only used and scores seen just once.

The official metric for DrivenData was classification rate (accuracy); however, class weights were included to improve performance against F1 score and provide a more useful real-world application where classification of the minority class (functional needs repair) would be essential.

**Final random forest 5-fold CV scores:** 99 features (7 numeric) with class weights
   - Accuracy 0.797
   - F1 0.791 micro, 0.679 macro
   - precision 0.792 micro, 0.722 macro
   - recall 0.797 micro, 0.658 macro

**Holdout** 
   - Accuracy: 0.802  
   - F1: 0.795 micro, 0.685 macro  
   - Precision: 0.796 micro, 0.725 macro  
   - Recall: 0.802 micro, 0.664 macro

## Tools
- Python and jupyter Notebook
- Numpy and Pandas for data manipulation
- Matplotlib and Seaborn for plotting
- SQLAlchony and SQLite
- 

## Communication
In addition to the slides and visuals presented, [Tanzania Waterpoints](https://public.tableau.com/profile/arjun#!/vizhome/TanzaniaWater/TanzaniaWaterpoints) will be embedded on my personal website and blog.
