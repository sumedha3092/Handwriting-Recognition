# Handwriting-Recognition

Write and submit your python codes in “Jupyter Notebook” to perform the following tasks. Make sure to provide proper descriptions as MarkDown for each section of your code.

A) Download the dataset “Digit” and its label from this link: https://app.box.com/s/sogk96kukv6ayyyy6ym63a2nu3aozif7
B) Build the feature matrix and label vector: Each image is considered as a data sample with pixels as features. Thus, to build the feature table you have to convert each 8x8 image into an array of 64 elements (i.e. 64 pixels), and put it as a row of the feature matrix with 64 feature columns.
C) Use sklearn functions to split the dataset into testing and training sets with the following parameters: test_size=0.1, random_state=2.
D) Use scikit-learn “Random Forest” classifier to recognize the hand-written digits based on the training/testing datasets that you built in part (c). Use this command to import and define your classifier:

from sklearn.ensemble import RandomForestClassifier

my_RandomForest =

RandomForestClassifier(n_estimators = 19, bootstrap = True, random_state=2)

Use my_RandomForest.fit for training your random forest classifier and my_RandomForest.predict for prediction. Test your Machine Learning Algorithm on testing set (from part(c)), and calculate and report the accuracy.
E) Write some codes to find which one of the data samples (i.e. which images) have been misclassified (classified incorrectly) in your testing set. Then, use the following command to show the misclassified images: plt.imshow(image_name, cmap=plt.cm.gray_r, interpolation='nearest')
