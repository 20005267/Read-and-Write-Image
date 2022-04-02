# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By: KAYALVIZHI M
### Register Number: 212220230024
# i) To Read,display the image
```python3
import cv2
color_image = cv2.imread("pikachu.jpg",1)
cv2.imshow('212220230024 , KAYALVIZHI',color_image)
cv2.waitKey(0) 
```
# ii) To write the image
```python3
import cv2
color_image = cv2.imread('pikachu.jpg',1)
w = cv2.imwrite('img.png',color_image)
cv2.imshow('212220230024 , KAYALVIZHI',color_image)
cv2.waitKey(0)


```
# iii) Find the shape of the Image
```python3

import cv2
import random
color_image = cv2.imread('pikachu.jpg',1)
print(color_image.shape)

```
# iv) To access rows and columns
```python3
import cv2
import random
color_image = cv2.imread('pikachu.jpg',1)
for i in range(100):
    for j in range(color_image.shape[1]):
        color_image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]

cv2.imshow('212220230024 KAYALVIZHI',color_image)
cv2.waitKey(0)



```
#  v) To cut and paste portion of image
```python3
import cv2
color_image = cv2.imread('pikachu.jpg',-1)
tag = color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212220230024',color_image)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

![read and display image](https://user-images.githubusercontent.com/75413726/161381455-2a38fad4-f75c-4eea-a11e-6bea0ac94ebb.jpg)


### ii) Write the image

![write the image](https://user-images.githubusercontent.com/75413726/161381467-bf8961ee-92b8-444a-b742-842007c44d29.jpg)


### iii) Shape of the Image

![shape of the image](https://user-images.githubusercontent.com/75413726/161381477-d4cdbc3b-1478-498c-a72d-8033c65e6012.jpg)

### iv) Access rows and columns

![access row and column](https://user-images.githubusercontent.com/75413726/161381487-d8d58f5d-132a-4177-938f-0a008ada1f61.jpg)

### v) Cut and paste portion of image

![cut and paste portion of image](https://user-images.githubusercontent.com/75413726/161381502-a6d2d238-d19a-4c4c-bb56-4cec2fbca5ec.jpg)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


