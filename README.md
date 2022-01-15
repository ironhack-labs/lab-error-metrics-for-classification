![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Lab | Error metrics for classification

In this lab, you will be using the [Sakila](https://dev.mysql.com/doc/sakila/en/) database of movie rentals. You have been using this database for a couple of labs already, but if you need to get the data again, refer to the official [installation link](https://dev.mysql.com/doc/sakila/en/sakila-installation.html).

<!-- The database is structured as follows:

<br>

![DB schema](https://education-team-2020.s3-eu-west-1.amazonaws.com/data-analytics/database-sakila-schema.png) -->

<br>

### Instructions

Work on the models that you created to predict the movie rating. 

1. Create a Python function named `get_model_metrics`, that given a model, the `train`, and the `test` sets, returns a pandas dataframe with the following columns: (`Error_metric`, `Train`, `Test`). The error metrics reported must be 
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Kappa
   - AUC
2. Use sklearn [classification_report](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.classification_report.html?highlight=report#sklearn.metrics.classification_report) to create another Python function, that given `y_train`, `y_train_pred`, `y_test`, `y_test_pred`, and a list of labels of the classes names,get a similar report for the `train` and the `test` sets.
3. Create a Python function named `plot_model_metrics`, that given a model, the `train`, and the `test` sets, will plot:
   - Confusion matrix
   - ROC curve
