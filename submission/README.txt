For our final submission:

Before running the submission.ipynb jupyter Notebook, ensure that there is a directory "all/" in the same root directory.
It should contain the file "model_1.h5"

Then, add the following files to the folder:
- train_images.npy (the public training data set) 
- train_labels.csv (the public training data set labels)
- test_images.npy (the private data set [NOT the public test data set!!])

The code will load the previously trained model and run on the private test data, outputting the results in submission.csv

= = = = =

If you would like to run our other code for reference:

LinearSVM:
Before running the baseline.ipynb jupyter Notebook, make sure the directory in which the .ipynb file is located contains 3 files: 
- scaled_train_images.npy
- scaled_test_images.npy
- train_labels.csv
Then, run the notebook, and the results will be output into submission.csv

-----

Feed-forward Neural Network:
Before running the neural_network.ipynb jupyter Notebook, make sure the directory in which the .ipynb file is located contains 3 files: 
- scaled_train_images.npy
- scaled_test_images.npy
- train_labels.csv
Then, run the notebook, and the results will be output into submission.csv

-----

Convolutional Neural Network: (This is the one we use for leaderboard competition)
Before running the CNN.ipynb jupyter Notebook, make sure the .ipynb file are locate in the direactory which has an "all" folder. 
In the all folder, it should contains 3 files: train_images.npy, test_images.npy and train_labels.csv
This code will read train files and test files. It will use train file to generate two .npy file in current directory. It uses 
train_data.npy to train the model and test_data.npy to make predicition. This code will also generate a history_1.txt to keep
track of training process. In addition, the code will generate two files named model_1.h5 and model_1.json. The trained model
are saved into these two files. Finally, the code will generate a submission.csv which contains the class predicition 
of the test_images.npy

-----

Explanation of files:

train_images.npy: contains the raw images used to test the model
train_label.csv: contains the corresponding labels for those images

test_images.npy: contains the raw images for which you would like to generate predictions

scaled_train_images.npy: contains the images used to train the model, but cropped.
scaled_test_images.npy: contains the images used to test the model, but cropped.





