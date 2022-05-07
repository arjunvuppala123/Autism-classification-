# Autism-classification-
# Team Members
| Name      | SRN |
| ----------- | ----------- |
| SVSC Santosh |  PES2UG19CS346  |
| Swati Maste     | PES2UG19CS419   |
| Venkata Krishnarjun Vuppala   | PES2UG19CS451       |

Problem Statement
In the current age, Autism Spectrum Disorder (ASD) is gaining its momentum faster than ever. Detecting autism traits through screening tests is very expensive and time
consuming.  Though a number of studies have been carried out using different techniques, these studies didn’t provide any definitive conclusion about predicting autism traits. This long time taken to diagnose autism is delaying the treatment and resulting in problems in later life of the child.
 

Solution:
With the advancement of artificial intelligence and machine learning (ML), autism can be predicted at quite an early stage.
This project aims at developing a Deep Learning based model to detect autism based on data collected from facial images and behavioural patterns of the children. This approach also makes use of Linear Classification based approach called SVM. SVM uses a dataset containing different characteristics majorly observed and known symptoms of autism. Since this is a Medical
Application based project, the system aims at concluding a result only when both the above techniques produce or predict the same result. In case of mismatch, the system asks to provide another image or retry so as not to provide any False positive or False Negative.

Design flow:
Step 1: Gathering datasets related to facial Image and behaviour characteristics
Step 2: Pre-processing image/features extraction
Step 3: Train the model
Step 4: Optimize the Model
Step 5: Test the model
Step 6: Evaluate the model

Modules Used:
1) Numpy
2) Open CV (cv2)
3) Matplotlib
4) Seaborn
5) TensorFlow
6) Keras
7) Sklearn

Implementation:
	a) Datasets: 
		Images: https://www.kaggle.com/datasets/cihan063/autism-image-data,
		Behavioral Characteristic Dataset: https://www.kaggle.com/datasets/fabdelja/autism-screening-for-toddlers
		Notes about the datasets:
		i) Images of the Autism Dataset Used include 2540 images out of which 1270 images belong to the autistic class and the other half 1270 images are non autistic class.
		ii) Includes 300 images belonging to the test part which can be used to determine the accuracy of the model
		iii) For the Behavioral Characteristic Dataset, there are 1054 records of both autistic and non-autistic class.
	b) Models used:
		Models used here are VGG16, MobileNetV2, VGG 19 in addition to SVM acting as a linear classifier. We make use of pre-trained CNN on an image dataset
	 and SVM on behavioural patterns dataset(CSV file).
            Among the three models used, MobileNetV2 was the best in terms of accuracy (maximum attained: 87%) and training time(less number of epochs were required for achieving satisfactory accuracy).
            The SVM model had an accuracy of 98% and a loss of 0.3.
