# DengAI-datadriven
This is a github repo which tries to get a better prediction for Dengue in DataDriven competition

https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread/page/81/

This is a combined work of :

* [Pasindu Senanayaka](https://github.com/PasinduSenanayake) 
* [Piyumi Rameska](https://github.com/rameshka)
* [Arunan Sugunakumar](https://github.com/arunans23)

In the final [submission](https://github.com/arunans23/DengAI-datadriven/blob/master/uomcse-pap-submission3.ipynb) we did, we have tested with multiple training models.
* Linear Regression
* KNN
* SVM
* Gradient Boosting
* Random Forest
* MLP

Out of these, radient boost does well for San Juan and SVM does well for Iquitos. When we made the submission we got a score of **20.0577**.

  With feature engineered dataset which was preprocessed by visualising the correlations, our goal was to find a good machine model which would better suit the scenario. We had to try on several machine learning models with several parameters. Most of the parameters we used were chosen by trial and error method. Also we got suggestions from driven-data community and we were able to create a good model. Some of the data preprocessing that are done are filling the missing values with mean values and normalizing the training data.

  The Regression Algorithms that provided good results were Linear Regression, KNN, SVM, Gradient Boosting, MLP and Random Forest. Out of these, Gradient Boosting, SVM and Random Forest were more promising. Since San Juan and Iquitos are different cities, they have different causes for dengue spreading. Hence we had to train models for them separately and produce results separately. We did not use all the features. We used only selected features and created some new that had more correlation with the number of total cases.

  In the models, the parameters we used were decided after testing with multiples values. For example we used estimators of values 10, 30, 100, 300, and 500 for gradient boosting and decided that 100 gives the best values. At the end, we found out that two different models give good results for each city. 
