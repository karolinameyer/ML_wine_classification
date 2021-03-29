# ML_wine_classification
Red wine classification problem. Using different models and tunning hyperparameters with GridSearchCV.

Two approaches:
 - wine_classification
 original target class: quality, values from 1 to 10
 - wine_classification_target_adjustment
 target class modification: only 2 quality classes bad/good
 
This dataset is not easy to classify because of too many insufficiently distinct target groups and unevenly distributed samples per class.
That is the reason why the first approach's models shows bad results.
Thus, in the second approach target group is modified for 2 classes: bad and good. Results are much better. Nevertheless there are still some drowbacks, there is a big inequality in number of samples per classes. Thus the recall and precission of good-quality class is to improve.
The best ML model here is xgboost.
