NECO Individual Project: Model Execution Instructions

CONTENTS OF ZIP FILE
MLP Implementation.ipynb        — Full MLP training notebook
SVM Implementation.ipynb        — Full Linear SVM training notebook

NECO Test MLP.ipynb             — Test notebook for MLP 
NECO Test SVM.ipynb             — Test notebook for SVM 

Submission_Files/
    mlp_best_weights.pt         — Trained MLP model weights
    svm_best_weights.pt         — Trained SVM model weights

    mlp_scaler.pkl              — Scaler fitted on MLP training data
    svm_scaler.pkl              — Scaler fitted on SVM training data

    mlp_train_losses.npy        — MLP training loss history
    mlp_val_losses.npy          — MLP validation loss history
    mlp_best_epoch.npy          — Best epoch for MLP

    svm_train_losses.npy        — SVM training loss history
    svm_val_losses.npy          — SVM validation loss history
    svm_best_epoch.npy          — Best epoch for SVM

    X_test.npy                  — Test set features (114 samples, 30 features)
    y_test.npy                  — Test set labels (114 samples)


DATASET
Breast Cancer Wisconsin (Diagnostic) dataset.
Available directly in scikit-learn — no external download required.
Loaded using: from sklearn.datasets import load_breast_cancer

TO EVALUATE THE MODELS (No Retraining Required)
Open:
- NECO Test MLP.ipynb
- NECO Test SVM.ipynb
Run all cells in each notebook.

These notebooks:
- Load the saved model weights from Submission_Files/
- Apply the correct scaler
- Evaluate performance on the test set
Output:
- Confusion matrices
- Accuracy, precision, recall, F1 score

TO REPRODUCE FULL TRAINING
Run:
- MLP Implementation.ipynb
- SVM Implementation.ipynb

These notebooks:
- Perform preprocessing and standardisation
- Run cross-validation and hyperparameter tuning
- Train the final models
- Save outputs to Submission_Files/