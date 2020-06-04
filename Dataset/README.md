## Dataset Description:
# What should I expect the data format to be?
The images are provided in DICOM format. This can be accessed using commonly-available libraries like ```pydicom```, and contains both image and metadata. It is a commonly used medical imaging data format.

Images are also provided in JPEG and TFRecord format (in the ```jpeg``` and ```tfrecords``` directories, respectively). Images in TFRecord format have been resized to a uniform 1024x1024.

Metadata is also provided outside of the DICOM format, in CSV files. See the ```Columns``` section for a description.

# What am I predicting?
You are predicting a binary target for each image. Your model should predict the probability (floating point) between 0.0 and 1.0 that the lesion in the image is malignant (the ```target```). 
In the training data, ```train.csv```, the value ```0``` denotes benign, and ```1``` indicates malignant.

# Files:
* train.csv - the training set
* test.csv - the test set
* sample_submission.csv - a sample submission file in the correct format

# Columns:
* image_name - unique identifier, points to filename of related DICOM image
* patient_id - unique patient identifier
* sex - the sex of the patient (when unknown, will be blank)
* age_approx - approximate patient age at time of imaging
* anatom_site_general_challenge - location of imaged site
* diagnosis - detailed diagnosis information (train only)
* benign_malignant - indicator of malignancy of imaged lesion
* target - binarized version of the target variable
