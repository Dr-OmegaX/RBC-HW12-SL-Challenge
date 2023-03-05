# RBC-HW12-SL-Challenge

## Supervised Learning Challenge Module
Note: All related development has been applied to a python notebook file within the "Starter_Code" folder

### Update Notes:
Following 3 amendments made to the "credit_risk_resampling.ipynb" file on 3.4.23 (Aligned with RBC-CG Comments):
1. Under Step 1 of "Predict a Logisitic Regression Model with Resampled Training Data" the following changes were made:
  a.    From:   rs_predictions = rs_loan_classifier.predict(X_resampled)
        To:     rs_predictions = rs_loan_classifier.predict(X_test)
  b.    From:   balanced_accuracy_score(y_resampled, rs_predictions)
        To:     balanced_accuracy_score(y_test, rs_predictions)
2. Under step 3 of "Create a Logistic Regression Model with the Original Data" the following changes were made:
  a.    From:   training_report = classification_report(y_test, loan_status_predictions)
        To:     training_report = classification_report_imbalanced(y_test, loan_status_predictions)
