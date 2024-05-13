# Pre-reqs
Tensorflow 2.0

# Train
To train the system it is necessary to download the GOTPD database from the following URL:

https://www.kaggle.com/lehomme/overhead-depth-images-people-detection-gotpd1

The Data have to be stored in GOTPD_DATABASE folder and divided in gaussianas, imagenes and validation folders, where we have the training set output images, the training set input images and the validation and test subsets, dividid in another gaussianas and imagenes subfolders.

Once you adapted the data to the folders system, you'll only have to run Train.py and the system will train and save the trained model in DPDnet.h5 (it only save the weights).

# Test
The repository stores a DPDnet trained model, it is only a demo model to provide a demonstration, so it won't report the optimal results of the system.
To test the only step needed its to run Test.py, and the system will load the demo sequence to show the results obtained with the proposed system.

# Sample Data
In the GOTPD_DATABASE/validacion/imagenes and GOTPD_DATABASE/validacion/gaussianas you will find an example test sequence that will load Test.py to show how the system works and compare prediction and groundtruth.
