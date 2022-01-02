### Parkinsons Disease Detection using Speech and Image Data

### Image
For the Image Part we have used a method of Deep Learning and computer
vision for Image classification of two target labels called healthy and
Parkinson’s. We have used Data augmentation and transfer learning and
fine tuning for the image classification part on various pre trained models
such as MobileNet, VGGNet etc... Since we had a very limited dataset of 30
Images for validation and 72 images for training purpose for both spiral
and wave drawings.
### Data Acquisition and Collection
The data for the study has been collected from Kaggle’s data repository
which was posted by K Scott Mader. The data acquisition process was
performed at the RMIT, University, Melbourne, Australia. For the data
acquisition procedure, 55 subjects were recruited were 28 subjects
belonged to the Control Group and 27 subjects from the Parkinson Group.
All the subjects were asked to take two tests namely the Spiral drawing test
and the Wave drawing test. The drawing of the spiral was captured using
an A3 size commercially used a tablet, where an A3 paper was placed over
the tablet and an ink pen was used to sketch the spiral and the wave. Figure
1 shows a sample of images that were obtained from the data acquisition
process.

![download (2)](https://user-images.githubusercontent.com/46704901/147869329-2d9a26c0-6ed3-4559-98e4-c37860ea69aa.png)
![download (4)](https://user-images.githubusercontent.com/46704901/147869324-a6ef380c-a159-4d7e-a4f1-38f5ebc27b86.png)
![parkinimage](https://user-images.githubusercontent.com/46704901/147869312-af022ced-7099-47ff-a65b-727a3a19f555.png)
![download (3)](https://user-images.githubusercontent.com/46704901/147869322-d4c393ec-a8b3-4c14-848a-83e5b3fda4d8.png)

### Data Pre-processing and Augmentation
The images used in the study were subjected to resizing and histogram
equalization. The images from the spiral sketches were resized to 256 px
width and 256 px height, whereas the wave sketches were resized to the
width of 256 px and height of 512 px. In the images that have been
collected for the study, it can be observed that the images lack contrast and
brightness and overall clarity. Therefore, contrast enhancement and
adjustment were performed over all the images using Histogram
equalization. For the preparation of images for training, all the images were
subjected to a static policy-based augmentation. As the number of images is
quite less in the dataset, therefore, the application of Deep Learning
algorithms such as CNN’s becomes quite difficult. Therefore to ingest some
synthetic samples in the training dataset and also to increase the diversity
in the dataset image augmentations were performed. Table 1 below show
the different image augmentation parameters which were applied to the
training data for wave and spiral sketched respectively. Moreover, Figure 3
shows the histogram equalized and augmented images of the training data
set from both wave and spiral sketches
![Screenshot (15)](https://user-images.githubusercontent.com/46704901/147869367-5bbbfc31-5aa3-47c0-b8aa-5b98c4960ae3.png)

### EXPERIMENT AND RESULT
After fine tuning, the model nearly reaches 88% accuracy on the validation
set. And now you are all set to use this model to predict if our patient has
Parkinson’s or not.

![Screenshot (16)](https://user-images.githubusercontent.com/46704901/147869474-5184dd70-3b34-4d08-bf30-edddfcffccab.png)
![Screenshot (17)](https://user-images.githubusercontent.com/46704901/147869477-f99bcded-9317-48b9-983e-0608de2a7852.png)


------------------------------------------------------------------------------------------------------------------------------

### Speech
One of the points to remember about data pre-processing for regression
analysis is multicollinearity. Our csv file consists of 755 instances and 700
plus columns of feature set. We cannot use this immensely big data to train
our machine learning model since there is a very high chance of over fitting.
So in order to reduce some of the unnecessary features we first of all found
out which are the most highly correlated features by plotting a heat map of
the data and we found around 364 of them to be highly correlated. All of
the 364 features were dropped from the original data and after that feature
selection algorithm was used.

### Dropping Highly Correlated Features
![download (5)](https://user-images.githubusercontent.com/46704901/147869518-5756ce75-c30a-425c-bb8c-d4ddca77d453.png)

### Feature Selection and Feature Importance
![download (6)](https://user-images.githubusercontent.com/46704901/147869529-0ef5df56-d9a2-4cb1-9bf7-6d8652e06bf3.png)

### Final Experiment Report
![Screenshot (18)](https://user-images.githubusercontent.com/46704901/147869569-a465ad1f-ffdc-460d-ba13-6c196b8df2cc.png)
