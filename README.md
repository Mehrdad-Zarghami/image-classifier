# image-classifier
Deploying a Computer Vision Model

# Data :  
### About Dataset
You are provided with a dataset containing images of different sports classes. The dataset is split into a training set and a test set. The training set consists of labeled images belonging to the following sports classes: cricket, wrestling, tennis, badminton, soccer, swimming, and karate. Each image is associated with a unique image ID and its corresponding class label. The test set contains unlabeled images for which you need to predict the class.

### Files
* train.csv - the training.csv file, which includes the image id and its class of columns
* test.csv - the test.csv file contains only image id columns

### Folders

* train - folder contains the images of train.csv files
* test - folder contains the images of test.csv files

### Download:
* https://www.kaggle.com/datasets/sidharkal/sports-image-classification/data


## Data Preprocessing
 Since there is no label for test data, I am going to split 20% of the labeled training data as a new test set. By this, I will ensure:
* No dependency on the unlabeled test.csv.
*  You can measure accuracy and fine-tune the model properly.


1. Split 80% of the data for training and 20% for validation/test.
2. Save the new split into train/ and val/ folders.
3. Modify the PyTorch Dataset class to use the split.

