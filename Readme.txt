Here are the steps to run the program:
During running of the program, you might be asked to install packages including but not limited to sk-learn, spark-sklearn package, pandas, metrics.
1. Go to the folder path project_folder/code
2. Move the data to project_folder /code/input
3. Extract features by running extract_features.sh
4. Confirm the features are saved in folder project_folder /code/features
5. Run train_models.py to train different models using different combo of classifiers and features
6 Run models_combine.r to combines results from different modesl in a way that optimizes the area under the ROC curve (AUC).
7. Find the results in folder project/code/submission

The following content expains what each source code do:
main interface:
models_combine.r: combines results from different modesl in a way that optimizes the area under the ROC curve (AUC).
train_models.py: train different models using different combo of classifiers and features
basic source code:
santander_preprocess.py: preprocess the raw data
tsne_features.py: produce tsne features 
pca_features.py: produce two PCA features (# of pca can be edited)
kmeans_features.py: produce kmeans features with 2-10 clusters
rgf.py: classification algorithm regularized greedy forest


