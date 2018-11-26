train_images.npy: it should contains the training images
train_label.csv: it should contains the label of the training images
test_images.npy: it should contains the images data which you want to make predicition of the class

LinearSVM:
Before running the baseline.ipynb jupyter Notebook, make sure the .ipynb file are locate in the direactory which 
contains 3 files: scaled_train_images.npy, scaled_test_images.npy and train_labels.csv
The code will take 2 pre-processed data and train_label.csv to generate result.

Feedforward Neural Network trained by back propagation:
Before running the neural_network.ipynb jupyter Notebook, make sure the .ipynb file are locate in the direactory which 
contains 3 files: scaled_train_images.npy, scaled_test_images.npy and train_labels.csv
The code will take 2 pre-processed data and train_label.csv to generate result.

Convolutional Neural Network: (This is the one we use for leaderboard competition)
Before running the CNN.ipynb jupyter Notebook, make sure the .ipynb file are locate in the direactory which has an "all" folder. 
In the all folder, it should contains 3 files: train_images.npy, test_images.npy and train_labels.csv
This code will read train files and test files. It will use train file to generate two .npy file in current directory. It uses 
train_data.npy to train the model and test_data.npy to make predicition. This code will also generate a history_1.txt to keep
track of training process. In addition, the code will generate two files named model_1.h5 and model_1.json. The trained model
are saved into these two files. Finally, the code will generate a submission.csv which contains the class predicition 
of the test_images.npy

Before running the submission.ipynb jupyter Notebook, make sure the .ipynb file are locate in the direactory which has an "all" folder. 
In the all folder, it should contains 4 files: train_images.npy, test_images.npy, model_1.h5 and train_labels.csv
This code is created for generating submission.csv when we already have the model saved as model_1.h5. So this code will load this 
model and compute the prediction by using this model. It will be more time efficient if we already have previously trained model saved. 
