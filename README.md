# customer-revenue-prediction

### chanllenge overview
In this competition, you’re challenged to analyze a Google Merchandise Store (also known as GStore, where Google swag is sold) customer dataset to predict revenue per customer. Hopefully, the outcome will be more actionable operational changes and a better use of marketing budgets for those companies who choose to use data analysis on top of GA data.

Sep 18    
Explore data and define base function

Oct 4    
Feature engineering strategies:    
  1. drop constant features(meanningless for prediction)    
  2. keep intersection features between train and test dataset(make train and test dataset consistent)    
  3. label encode categorical features    
  4. fill na in numerical features as zeros and convert them to float    

Things to do to improve model performance(advance feature engineering):       
  1. one-hot-encode categorical features(make them as 'dummy' variables)    
  2. normalize numerical features(assumption)    
  3. find smarter way to select features(feature selection techniques such as Foward Selection, model based selection, etc.)  
  4. featrues imputation(add more featrues that compute from one or more featrues)
  
  Oct 8    
  The competition is based on time series. Figure out the techniques to build model based on time series
  
  Oct 9    
  Based on the other authors' kernel, it is better to divide the task to session level and visitor level. As for session level, it is essential to include the time to next session as a new features, which has been proved useful for the time series prediction task. The rmse of CV score becomes better after features including time to next session. 
