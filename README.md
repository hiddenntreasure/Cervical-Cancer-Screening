# Cervical-Cancer-Screening
Competition arranged by Kaggle

## 1.Problem Description:

AI is largely used in Medical sector.In near future, AI will take an important part almost in all sectors.

Colposcopy is used to detect cervical cancer/cin/lession . In this problem image of three different class and need to learn from images and predict class of unseen images.

## 2.Dataset: 
 
It contains almost 5000 images of three different class.And 512 images for test dataset.

But as i didn't take part in the competition.Because it happened in 2016. I am trying to solve in 2020. 

I don't take all 5000 images. I took only 2300 images as train data and 150 images for validation of  each classe.

## 3. Images preprocessing:

Images had unwanted region which don't require. So,crop images manually using domain knowledge about the task. Or use image segmentation approach. Image segmentation by creating mask/annotation using domain knowledge and apply U-Net apporach.Or simply use max Hist algo. As image's most of the part is required for classification. Using Max Hist will automatically segment ROI.

## 4. Model:

| Model | Fine Tune | Epoch | Training Accuracy | Validation Accuracy | Loss |
| --- | --- | --- | --- | --- | --- |
| VGG19 | No | 68 | 83 | 72 | 0.2678 |
| VGG19 | block-5 Conv-1 | 88 | 87 | 50 | 0.58 |
| DenseNet201 | No | 43 | 80 | 65 | 0.4257 |
| DenseNet201 | block-21 conv-5 | 137 | 68 | 72 | 0.25 |
