# Machine-Learning-and-International-Rural-Water-Supply
(Major Project)

This Project cantains of the final thesis (Dissertation). 

This repositart consist of the code used to detect corrosion from the parts of the pump in the sub-saharan Africa.

The first step in any project is the collection of data. Data for this project was
provided by the BGS. The data provided was in the form of high dimensional images. 




Although these images were not taken specifically for this project. These images were part of the hidden crisis project. After the images were received, the second step was the analysis of the data. As the data provided is very small in number. The analysis was a basic but important step. In total after analysis, 746 images were gathered. In the 746 images, the count of the corroded images was more in comparison to the non-corroded. To balance the dataset more images from the non-corroded label were chosen. But these images still couldn’t be used for the training purpose. A lot of the images from this data set were carrying unwanted information, which could lead to lower accuracy. All these images were made entitled for the task by performing data curation on it. In the step, data curation all the images were manually one by one cropped using software GIMP 2.0. This process took more than a week to manually crop all the important information from the image. Further, after all the image were given name from the CSV file given by using a python script. This script further added the corroded or non-corroded to the name of the image on the basis CSV file. This helped in assigning the label ahead in the code. After the name was changed for all the images, all these images were further resized. Data Augmentation was also performed on these images to increase the dataset. All these images were saved in the numpy array according to the size taken by the neural network as input. Not only images but labels were also saved in the numpy array. All the corroded images where given label 1 and non-corroded images were given label 0. All these images where then feed to the neural network for the production of important features. These important features were then further given as the input to the classifier. In the model, PCA, and SVD were also used just before the classifier. But somehow they were not able to make accuracy better. The result for it are in the next section. Just like the PCA and SVD, Data Augmentation was not able to generate better accuracy. One of the reasons behind the failure of the data augmentation was, almost all images are having pipes. By increasing the image, it got affected by the overfitting which resultant poor accuracy.
