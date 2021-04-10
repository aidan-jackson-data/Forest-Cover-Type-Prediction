Final-Project---Forest-Cover-Type-Prediction
====================================================

<img align="right" width="180" src="./images/berkeley.png"/>

#### Authors: [Aidan Jackson](https://github.com/aidan-jackson-data) | [Andi Morey](https://github.com/andimorey) | [Naga Chandrasekaran](https://github.com/nagachandrasekaran) | [Scott Gatzemeier](https://github.com/sngatzemeier) | 
#### Instructor: D. Schioberg, PhD <br> 
U.C. Berkeley, Masters in Information & Data Science program - [datascience@berkeley](https://datascience.berkeley.edu/) 

Spring 2021, W207 - Machine Learning - Wed. 6:30pm PDT

## Description

This repo contains itterative solutions (including a final solution) for the [Kaggle Forest Cover Typer Prediction](https://www.kaggle.com/c/forest-cover-type-prediction) challenge, developed by Aidan Jackson, Andi Morey, Naga Chandrasekaran, and Scott Gatzemeier.  The goal of this project is to classify trees in four different wilderness areas of the Roosevelt National Forest in Northern Colorado. These areas represent forests with minimal human-caused disturbances, so that existing forest cover types are more a result of ecological processes rather than forest management practices. Accurate results of a successful model will allow US Forest Service (USFS) to predict the predominant cover type trees to plant in reforestation efforts of the 800,000 acres in the Roosevelt National Forest.  

Our solution leverages a variety of modeling techniques.  Base models were developing using K-Nearest Neighbors, Naive-Bayes, Logistic Regression, Decision Tree, and Neural Networks.  These models were itteratively improved independently through data cleansing/formating, feature engineering, and hyperparameter tuning.  These models were then leveraged to build an ensemble model for our final results.

#### Highlight of key files included in this repository:

  |Folder | File | Description |
  |:----|:----|:------------|
  |.. | [207-final-notebook.ipynb](207-final-notebook.ipynb) | Jupyter Notebook containing the final write up of our report.|
  |presentations | [Midterm_Pres_Forest_Cover_Type_Prediction](/presentation/Midterm_Pres_Forest_Cover_Type_Prediction.pdf) | Midterm presentation of EDA and initial models|
  |data | [covtype.csv](covtype.csv) | Raw Dataset containing test and training data, Number of Records: 581012 and Number of Features: 55|
  |data | [test.csv](test.csv) | Test dataset, Number of Records: 565892 and Number of Features: 55 |
  |data | [train.csv](train.csv) | Dataset used to train models, Number of Records: 15120 and Number of Features: 56|

> Add more after complete
  
  ## Performance 
  
> Section to be updated when we are complete
 
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
  
  
