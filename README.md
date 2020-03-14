# Brain_hemorrhage_detection
Brain hemorrhage detection based on CT images of the head. 

Images used for this project were open-source CT images of the head found on Kaggle. There are 100 normal images and 100 images with brain hemorrhage in the dataset. 

After exploratory analysis, all images were resized to 128x128 pixels. Because of lack of data, image augmentation was used during training. Classification was accomplished using a CNN built in Keras. 

Since this is a medical task, in order to avoid false negatives the original dataset was artificially expanded to include more images with brain hemorrhage. By doing this the network favored positive results and ended up predicting zero false negative results. This didn't disrupt the networks accuracy and it didn't predict more false positives then previous.
