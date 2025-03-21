## Naive Bayes Classifier

### Make sure your repo is up-to-date

Assignment code is pushed weekly during the semester, so please pull from this repo first and copy the NaiveBayes folder to your repo. Also note that in the data directory, the audiology_train.csv and audiology_test.csv have different names than before (they did not have a .csv file extension), so be sure to copy those over to your data directory.

### In the data, do NOT treat "?" as missing values in this assignment. Treat it as a regular value that feature X can take.

### Build your own categorical Naive Bayes classifier

#### Implement my_NB.fit() function in [my_NB.py](NaiveBayes/my_NB.py)
Inputs:
- X: pd.DataFrame, independent variables, each value is a category of type str.
- y: list, np.array or pd.Series, dependent variables, each value is a category of type int or str.

#### Implement my_NB.predict() function in [my_NB.py](NaiveBayes/my_NB.py)
Input:
- X: pd.DataFrame, independent variables, each value is a category of type str.

Output:
- Predicted categories of each input data point. List containing elements of type str or int.

#### Implement my_NB.predict_proba() function in [my_NB.py](NaiveBayes/my_NB.py)
Input:
- X: pd.DataFrame, independent variables, each value is a category of type str.

Output:
- Prediction probabilities of each input data point belonging to each categories. pd.DataFrame(list of probabilities, columns = self.classes_).

### Test my_NB classifier with [A5.py](NaiveBayes/A5.py)
Expected output:
```
(base) NaiveBayes % python A4.py 
cochlear_age    0.999408
cochlear_age    0.999408
cochlear_age    0.875175
cochlear_age    0.484233
cochlear_age    0.992703
cochlear_age    0.997401
cochlear_age    0.998318
cochlear_age    0.998318
cochlear_poss_noise     0.902857
cochlear_unknown        0.611369
mixed_cochlear_unk_fixation     0.832907
mixed_cochlear_unk_fixation     0.755148
normal_ear      0.507668
normal_ear      0.990685
cochlear_age    0.997749
cochlear_age    0.992896
normal_ear      0.997311
mixed_cochlear_unk_fixation     0.930178
cochlear_age    0.982908
cochlear_age    0.996372
cochlear_age    0.959620
mixed_cochlear_unk_fixation     0.397127
normal_ear      0.997311
mixed_cochlear_unk_fixation     0.983080
cochlear_age_and_noise  0.619968
cochlear_poss_noise     0.601495
```

### Do not forget to push your local changes to the Github server.

 
 ## Grading Policy 
 - Importing additional packages that implement Naive Bayes, such as sklearn, is not allowed.
 - 4 (out of 7) points will be received if A4.py successfully runs and makes predictions.
 - The 3 remaining points will be given based on the percentage of the same predictions with the correct implementation.
 
  
## Hint
 - If you would hints or to figure out how to get started, you can use [my_NB_hint.py](NaiveBayes/my_NB_hint.py).
 - [my_NB_hint.py](Naive Bayes/my_NB_hint.py) has the predict() and predict_proba() functions already implemented. You will only need to complete the fit() function.
 - If you use the hint file, remember to rename it as my_NB.py before submitting.
