Random Forest is an ensemble learning method that builds **multiple decision trees** and combines their predictions to improve accuracy.
- Each tree is trained on a **random subset of the data and features**
- This randomness makes the trees **different from each other**
- Each tree makes a prediction, and the final output is decided by **majority voting**


Step 1: Bootstrapping
Choose random subsets of the original dataset with replacement so that 	the total number of  rows in the selected subset is the same as the original 	dataset

Step 2: 
Randomly select a subset of features for each dataset. The number of 	selected features is a hyperparameter usually set to the square root or log of the total number of features. **Hyperparameter** is the number of subsets.

Step 3:
Train one tree for each selected dataset and set of features.

Step4: 
For new unseen data, make predictions using the majority voting.
