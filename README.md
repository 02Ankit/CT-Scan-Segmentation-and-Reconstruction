# CT-Scan-Segmentation-and-Reconstruction 
        Abhijeet Dewangan September 29, 2022
### Artificial Intelligence for Medical Image Analysis

Q1
Task: Calculation of Infection Rate from given expert annotations and classify CT Scan slices into three categories: Normal, Mild and Severe.
The distribution I obtained is: Distribution in terms of percentage:
Normal: 40.546%, Mild: 54.980%, Severe: 5.474%


![1a1](https://user-images.githubusercontent.com/67556459/220041806-caa990a8-3359-4ace-b183-43eeba720bbb.png)
### Sample slices for each categories are:
![1a2](https://user-images.githubusercontent.com/67556459/220043069-0b099cb1-d723-4f05-9260-e30db501145f.png) 
![1a3](https://user-images.githubusercontent.com/67556459/220043096-ccda9f15-fd79-4028-bfd1-450d890e003b.png) 
![1a4](https://user-images.githubusercontent.com/67556459/220043128-44c1e7e4-d2f2-4400-8f56-b959ea1baa7c.png)

Q2
Task: Used k-means clustering to segment CT scan images into background, infection and healthy region.
Evaluated the performance of segmentation using average dice score, sensitivity, specificity, and accuracy of infection and healthy regions.
The following results(averaged over all the samples) were obtained():

| - |Infection Region | Healthy Region |
|:--:|:-----------------:|:---------------:|
|Dice Score	|0.2062	|0.8559|
|Sensitivity	|0.5444	|0.7853|
|Specificity	|0.9780	|0.9959|
|Accuracy	|0.9730	|0.9709|

###### Average evaluation metrics for infection and healthy region.

### Two sample slices with Expert Annotation(left), Predicted Infection Mask(Middle) and CT Scan(Right)

![1b0](https://user-images.githubusercontent.com/67556459/220049319-0eeefbf2-b702-4709-8432-1501af4789d6.png)

Q3
Task: Reconstructed CT Scan images from limited angle Sinogram(4x and 8x). Evaluated the performance of reconstruction using PSNR and SSIM.
Further, performed segmentation using k-means and evaluated the performance as done in part 2.
| - |4x Reconstruction | 8x Reconstruction |
|:--:|:-----------------:|:---------------:|
|PSNR	|5.6857	|4.9811|
|SSIM	|0.1452	|0.1124|

###### PSNR & SSIM for Reconstructed CT Scan Images.
Sample slices for reconstruction using 4x(left), 8x(middle) limited angle Sinogram and Ct Scan(right).

![1c1](https://user-images.githubusercontent.com/67556459/220050467-7c4fa263-5951-4a04-ae37-a421d2c5bcd2.png)

## Repeat Q2 for Reconstructed Images.
Evaluation of Image Segmentation for Reconstructed CT Scan images.
(i)	4x Reconstruction Evaluation
| - |Infection Region | Healthy Region |
|:--:|:-----------------:|:---------------:|
|Dice Score	|0.2731	|0.8235|
|Sensitivity	|0.4169	|0.5432|
|Specificity	|0.9465	|0.9897|
|Accuracy	|0.9633	|0.9814|

###### Average evaluation metrics for infection and healthy region for reconstructed CT Scan images from limited angle Sinogram(4x).

Two Sample Slices

![1c2](https://user-images.githubusercontent.com/67556459/220051696-7880a93c-b85f-4464-9ea0-310547aec869.png)

(ii)8x Reconstruction

Evaluation

| - |Infection Region | Healthy Region |
|:--:|:-----------------:|:---------------:|
|Dice Score	|0.2015	|0.6125|
|Sensitivity	|0.3645	|0.5019|
|Specificity	|0.9592	|0.9915|
|Accuracy	|0.9622	|0.9871|

###### Average evaluation metrics for infection and healthy region for reconstructed CT Scan images from limited angle Sinogram(8x).

Two Sample Slices

![1c3](https://user-images.githubusercontent.com/67556459/220052541-d6c3d3ec-efa8-48f5-907b-c10eb25f72dc.png)

