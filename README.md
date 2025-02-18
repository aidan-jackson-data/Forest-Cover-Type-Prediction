Final-Project---Forest-Cover-Type-Prediction
====================================================

<img align="right" width="180" src="./images/berkeley.png"/>

#### Authors: [Aidan Jackson](https://github.com/aidan-jackson-data) | [Andi Morey Peterson](https://github.com/andimorey) | [Naga Chandrasekaran](https://github.com/nagachandrasekaran) | [Scott Gatzemeier](https://github.com/sngatzemeier) | 
#### Instructor: D. Schioberg, PhD <br> 
U.C. Berkeley, Masters in Information & Data Science program - [datascience@berkeley](https://datascience.berkeley.edu/) 

Spring 2021, W207 - Machine Learning - Tue. 6:30pm PDT

## Description

This repo contains iterative solutions (including a final solution) for the [Kaggle Forest Cover Type Prediction](https://www.kaggle.com/c/forest-cover-type-prediction) challenge, developed by Aidan Jackson, Andi Morey, Naga Chandrasekaran, and Scott Gatzemeier.  The goal of this project is to classify trees in four different wilderness areas of the Roosevelt National Forest in Northern Colorado. These areas represent forests with minimal human-caused disturbances, so that existing forest cover types are more a result of ecological processes rather than forest management practices. Accurate results of a successful model will allow US Forest Service (USFS) to predict the predominant cover type trees to plant in reforestation efforts of the 800,000 acres in the Roosevelt National Forest.  

Our solution leverages a variety of modeling techniques.  Base models were developing using K-Nearest Neighbors, Naive-Bayes, Logistic Regression, Decision Tree, and Neural Networks.  These models were iteratively improved independently through data cleansing/formatting, feature engineering, and hyperparameter tuning.  These models were then leveraged to build an ensemble model for our final results.

#### Highlight of key files included in this repository:

  |Folder | File | Description |
  |:------|:-------|:------------|
  |.. | [207-final-notebook.ipynb](207-final-notebook.ipynb) | Jupyter Notebook containing the final write up of our report.|
  |Models | [Individual Model Notebooks](/Models/) | Folder containing principal component analysis, individual model testing and ensemble model.  Each folder include the respective notebooks and results.  Models test include: Naive Bayes, Logistic Regression, Neural Network, Decision Trees, K-Nearest Neighbor, Gaussian Mixture Models, and finally the bagging ensemble. |
  |EDA | [Individual EDA Notebooks](/EDA/) | Exploratory Data Analysis notebooks to help with model hyperparameter tuning and feature engineering
  |presentations | [Midterm_Pres_Forest_Cover_Type_Prediction](/presentations/Midterm_Pres_Forest_Cover_Type_Prediction.pdf) | Midterm presentation of EDA and initial models|
  |presentations | [Final Presentation - Cover Type Prediction](/presentations/W207%20Final%20Report_%20Forest%20Cover%20Type%20Prediction.pdf) | Final Presentation with Ensemble Model |
  |data | [covtype.csv](covtype.csv) | Raw Dataset containing test and training data, Number of Records: 581012 and Number of Features: 55|
  |data | [test.csv](test.csv) | Test dataset, Number of Records: 565892 and Number of Features: 55 |
  |data | [train.csv](train.csv) | Dataset used to train models, Number of Records: 15120 and Number of Features: 56|
 
  ## Performance 
  
Tuned & Featured Engineered Model Results
|Model|Kaggle Accuracy, Before (%)|Kaggle Accuracy, After (%)|
|:-----:|:----:|:----:|
| K-Nearest Neighbor | 63 | 71 |
| Naive Bayes | 42 | 42 |
| Logistic Regression | 40 | 59 |
| Decision Tree | 66 | 75 |
| Neural Network | 35 | 72 |
| Tie Breaker Model | - | 72 |
|Ensemble| 67 | 79 |

### Final Ensemble Kaggle Accuracy: 79.579%
#### Best Leaderboard Position: 197 / 1693
> The final ensemble is found to have an accuracy almost to 80%. With this best accuracy, the final leaderboard position would have been 197 out of 1693 had this team entered, breaking the top 15%.
 
  ## Data and Challenge Description
The study area includes four wilderness areas located in the Roosevelt National Forest of northern Colorado. Each observation is a 30m x 30m patch. We were asked to predict an integer classification for the forest cover type. The seven types are:

> 1. Spruce/Fir
> 2. Lodgepole Pine
> 3. Ponderosa Pine
> 4. Cottonwood/Willow
> 5. Aspen
> 6. Douglas-fir
> 7. Krummholz

The training set (15120 observations) contains both features and the Cover_Type. The test set contains only the features. The challenge was to predict the Cover_Type for every row in the test set (565892 observations).
  
  
