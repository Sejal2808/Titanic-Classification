# Titanic-Classification
A machine learning model on the `Titanic dataset` to predict whether a passenger on the Titanic would have been survived or not using the passenger data. If you want more details then click on **[link](https://www.kaggle.com/c/titanic)**.

So the data has information about passengers on the Titanic, such as `name` , `sex`, `age`, `survival`, `economic status(class)`, etc.

## Data Visualisation
>Making the count plot for Survived

![Survived](https://user-images.githubusercontent.com/123626918/227458583-bafe1c4b-ea9e-4a9e-a804-f8ceaf7d0a1a.png)

![Sex](https://user-images.githubusercontent.com/123626918/227459561-95c84452-f183-4bfb-bc75-bec7f4673f42.png)

![Sex-Survived](https://user-images.githubusercontent.com/123626918/227459824-2dea3adc-f7aa-42a8-8140-770d1b0266d4.png)

![Pclass](https://user-images.githubusercontent.com/123626918/227459977-b66fdbbc-7db1-41d6-a870-fa2954c1634b.png)

![Pclass-Survivors](https://user-images.githubusercontent.com/123626918/227460086-c4d10af7-9d28-45db-867e-b675259ea800.png)


## Model Training
```bash
model = LogisticRegression()
#training the Logistic Regression model with training data
model.fit(X_train, Y_train)
```
## Model Evaluation
>Accuracy Score for Training data
```bash
training_data_accuracy = accuracy_score(Y_train, X_train_prediction)
print('Accuracy score of training data : ', training_data_accuracy)
```
**Accuracy score of training data :** 80%  <!--~~(0.8075842696629213)~~-->


>Accuracy Score for Testing data
```bash
test_data_accuracy = accuracy_score(Y_test, X_test_prediction)
print('Accuracy score of test data : ', test_data_accuracy)
```
**Accuracy score of test data :** 79 %   <!--(0.7821229050279329)-->

## License

[MIT](https://choosealicense.com/licenses/mit/)
