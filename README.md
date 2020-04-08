# FinalProject
Final Project

1)  Research question:   Skin cancer is the most common human malignancy, is primarily diagnosed visually, beginning with an initial clinical screening and followed potentially by dermoscopic analysis, a biopsy and histopathological examination. Automated classification of skin lesions using images is a challenging task owing to the fine-grained variability in the appearance of skin lesions. This the HAM10000 ("Human Against Machine with 10000 training images") dataset.It consists of 10015 dermatoscopicimages which are released as a training set for academic machine learning purposes and are publiclyavailable through the ISIC archive. This benchmark dataset can be used for machine learning and for comparisons with human experts.

2)  Domain and Data: 
    Source of Data - https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000
    Domain - Health, Image Data
    Size of Data : HAM10000_matadata.csv - This file has 7 columns with 10015 rows. This has information about patient details.
          In addition to this file we have 10015 images of various skin cancer patients. We also have hmnist*.csv files which has pixel           information.

    Preprocessing: We have removed nulls from the age column and replaced it with the mean.
                   We added 3 new columns in the table for better understanding of the data.
                   1) With dx - Cancer Type
                   2) With dx-  Cancer Id
                   3) Age Range - Age - For Plotting age Data

         
       ![image](https://github.com/Group13-KBS/FinalProject/blob/master/Tablesummary.JPG)
       
    Dashboard:
    
    
       
      

      c)  tentative plan for analysis on GCP

           1)  EDA and Preprocessing:
               a. We will plot graphs based on the skin lesion type.
               b. Plotting of Technical Validation field (ground truth) which is dx_type to see the distribution of its 4 categories
               c. Plotting the distribution of localization field.
               d. Also analyze patient informationd details.
               We can work on the preprocessed data and implement the recommendation algorithm.

           2)  Dashboard for User group, Dashboard for Data Engineers:
               We will plan to represent graphically the different types of skin lesions based on images. Also dashboards for the                      skin images occured based on various factors.
           3)  GCP further processing :
               We will use classiffication algorithms(CNN) to predict the skin lesion.

           4)  Evaluation of results :
               We will be evaluating our result by categorical cross entropy. The smaller the value more accurate result will                          be. We will try to implement and tune the algorithm to get the least categorical cross entropy.          

           5)  Steps for production model :
               We will load our data in Classification model and train our model with partial data and check categorical cross entropy .                After training , we will be testing our model and prepare the model for Production data.

           6)  Final Dashboard for User Group :
               Finally, we can recommend users the chances of skin cancer based on the images . Our model can be used for machine                      learning and for comparisons with human experts.
