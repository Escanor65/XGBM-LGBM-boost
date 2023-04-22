# XGBM-LGBM-boost
This code snippet is an example of building classification models using XGBoost and LightGBM libraries. The dataset used for this task is the Pima Indians Diabetes dataset, which contains medical information of female patients, and the objective is to predict whether or not the patient has diabetes.

The code is divided into two sections. The first section builds an XGBoost model and the second section builds a LightGBM model.

For the XGBoost model, the code starts by loading the dataset using the loadtxt function from NumPy. The data is then split into input features (X) and target variable (Y). The train_test_split function from scikit-learn is used to split the data into training and testing sets. Then, an instance of the XGBClassifier class is created and trained on the training data. The trained model is then used to make predictions on the testing data, and the accuracy of the model is calculated using the accuracy_score function from scikit-learn.

For the LightGBM model, the code starts by loading the dataset using the read_csv function from pandas. Then, the data is split into input features (X) and target variable (Y) using the iloc method. The train_test_split function is used to split the data into training and testing sets. Next, an instance of the lgb.Dataset class is created using the training data. The parameters for the LightGBM model are defined in the params dictionary, and the train function from LightGBM is used to train the model. The trained model is then used to make predictions on the testing data, and the accuracy of the model is calculated using the accuracy_score function from scikit-learn.

Both models use similar approaches and achieve similar results. However, the parameters and methods used in each library may differ, and it is important to tune them to achieve the best performance for a specific dataset.
