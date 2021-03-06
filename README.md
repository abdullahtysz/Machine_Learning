# Machine_Learning


# Machine_Learning Steps

--- Exploratory Data Analysis and Visualization

---### Machine Learning

-- Train | Test Split 
➊ X_train, X_test, y_train, y_test = train_test_split()

-- Scalling (if needed) ( değişkenleri  belirlediğimiz aralıklara indirgiyoruz, KNN-SVM-KMeans), 
➊ scaler = scaler_name()
➊➋ scaler.fit_transform(X_train)
➊➋➌ scaler.transform(X_test)

-- Modelling( eğitim)
➊ model = model_name().fit(X_train, y_train)
➊➋ y_pred = model.predict(X_test)
➊➋➌ y_pred_proba = model.predict_proba(X_test)

-- Model Performance (metrics)
➊ Regression		=> r2_score, MAE, MSE, RMSE
➊➋ Classification		=> accuracy, recall, precision, f1_score (confusion_matrix, classification_report)
➊➋➌ Cross Validate	=> cross_val_score, cross_validate ( ml modelinn görmediği veriler üzerinden)

-- Tunning (if needed) 
➊ grid_param = {}
➊➋ GridsearchCV(grid_param)

-- Final Model
➊ model = model_name().fit(X, y)
-- Model Deployment
