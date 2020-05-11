# Cervical-Cancer-Screening
Competition arranged by Kaggle

## 1.Problem Description:

AI is largely used in Medical sector.In near future AI will take an important part almost in all sectors.

Colposcopy is used to detect cervical cancer/cin/lession . In this problem,we get image of three different stage. We need learn from images of three class and predict class of unseen images.

## 2.Dataset: 
 
It contains almost 5000 images of three different class.And 512 images for test dataset.

But as i didn't take part in the competition.Because it happened in 2016. I am trying to solve in 2020. 

I don't take all 5000 images. I took only 2300 images as train data and 150 images for validation of  each classe.

## 3. Images preprocessing:

Images had unwanted region which don't require to learn unique  pattern. So,crop images manually using domain knowledge about  the task. Or could use image segmentation approach. Image segmentatio could  do by creating mask/annotation using domain knowledge or simply use max Hist algo. As images most of the part is required for classification. Using the theme Max Hist will automatically segment ROI.
