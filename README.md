# Color-Correction-for-Color-blind-People-Graduation-Project

#                                                 Graduation Project is Achromatopsia Driver Assistance System (ADAS)
                                             
**The main solution in the color blindness system is to build a color correction sub-system for people with color blindness.**

This is done in two steps: the first is to simulate the problem and gather data, second is to build a deep learning model for color correction to be used.

## Problem and how we solved it
### Simulation the problem

![image](https://user-images.githubusercontent.com/48545560/181923632-22d3d691-5797-4d1d-94f6-c3aa37ae544e.png)

### The Color corrected Image

![image](https://user-images.githubusercontent.com/48545560/181923686-730d0495-54e9-4f6e-8a1a-df6bf1aca12a.png)


## Datasets Stage:

First, We worked on 9500 images from different environments collected by capture videos on the street by ourselves and using online adas datasetes (called Original Image).

Second, Applied the custom simulator to this dataset to generate dataset with corrected colors (called Target Images).

Third, Applied these 2 datasets to the Pix2Pix model which is an image to image translation architecture. We need to prepare the dataset to be paired images (one image contains the original version and the corrector image of the same image) as shown below figure.

![image](https://user-images.githubusercontent.com/48545560/181936549-889eb6ef-38eb-46df-8024-c162be0a4ba1.png)

All dataset and results we  have uploaded to google drive while working on it on this link: 
https://drive.google.com/drive/folders/1c6FK3TvBSq8YqB46kcuSzHV-8pH25Rew?usp=sharing


## AI Model Stage
                                   
The solution for correction images for people with colorblindness is a GANs Model. we used a deep learning model called Pix2Pix which divides to 2 sub models: Generator and Discrimiator.

The below diagram shows how pix2pix works.

![image](https://user-images.githubusercontent.com/48545560/181922408-a448a9db-f25a-408e-a9b9-35deb63c6496.png)

## The result is to succeed in converting the live stream of cameras to a color-corrected stream which is suitable for color-blind people to recognize the front objects while driving.

![image](https://user-images.githubusercontent.com/48545560/181937587-0615e8ba-69cd-4bb4-8cfa-99704e82b626.png)

![image](https://user-images.githubusercontent.com/48545560/181937574-60163895-f14d-4dda-89bf-83685ff736c9.png)

