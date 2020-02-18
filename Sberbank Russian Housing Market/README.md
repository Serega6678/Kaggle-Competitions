## Sberbank Russian Housing Market evaluation

**Work in progress**

Competition page: https://www.kaggle.com/c/sberbank-russian-housing-market

**Notebooks:**

1. **Sqaure_Analysis.ipynb** - full_sq, life_sq and kitch_sq NANs are filled in, incorrect data becomes more sensible after pipeline processing.

2. **Secondary_Features_Analysis** - build_year, floor, max_floor, num_room were filled; all features, coresponding to distance to smth are proved to be correct (judging by geolocation & mean value among the sub area), all the missing values were recovered where possible.

3. **Hyperparameters_tuning** - last NaNs in test data were filled in, data was normalized, categorical features were imputed and transformed into numbers, best hyperparametes were found

4. **Feature_selection** - final pipeline (capable of working with train, test and user's data) completed, the plan is to finish feature selection with greedy algorithm (take features which increase performance and then remove all of those features which were taken earlier and don't seem to improve performance and more) and different dimensionality reducton methods.

5. **Economics_analysis (Not done yet!)** - analysing prices reactions to micro and macro economics data to adjust price_doc in train to match the economy state and to make prediction independant from the current date.