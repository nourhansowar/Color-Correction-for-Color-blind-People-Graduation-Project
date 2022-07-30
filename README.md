# Color-Correction-for-Color-blind-People-Graduation-Project

#                                                 Graduation Project is Achromatopsia Driver Assistance System
                                             
*The main solution in the color blindness system is to build a color correction sub-system for people with color blindness.*

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


## AI Model Stage
                                   
The solution for correction images for people with colorblindness is a GANs Model. we used a deep learning model because it will be very fast in terms of processing time in the tools, we used like JESTSON board. 
After research in GANs architecture that used in image translation
specially colorblindness correction methods, we found that pix2pix architecture is the best
architecture for our project as also it is used in colorization old images.


![image](https://user-images.githubusercontent.com/48545560/181922408-a448a9db-f25a-408e-a9b9-35deb63c6496.png)
