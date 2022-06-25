### EX NO : 01
### DATE  : 01.04.2022
# <p align="center">READ AND WRITE AN IMAGE</p>
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

<br/>
<br/>
<br/>
<br/>

## Program:

```python

# Developed By: Aishree Ramesh
# Register Number: 212220230003

# To Read,display the image

import cv2
image_1=cv2.imread("pic_1.PNG")
image_2=cv2.imread("pic_2.PNG")
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)
cv2.imshow("pic_2",image_2)
cv2.waitKey(0)

# To write the image

cv2.imwrite("pic_1",image_1)
cv2.imwrite("pic_2",image_2)

# Find the shape of the Image

print(image_1.shape)
print(image_2.shape)

# To access rows and columns

for i in range(70,90):
    for j in range(110,170):
        image_2[i][j]=[0,0,0]
cv2.imshow("pic_2",image_2)
cv2.waitKey(0)

# To cut and paste portion of image

image_1[200:220,110:175]=image_1[70:90,110:175]
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)

```

<br/>
<br/>
<br/>
<br/>

<br/>
<br/>
<br/>
<br/>
<br/>


## Output:

### i) Read and display the image
![image](https://user-images.githubusercontent.com/70213227/161099189-bbacf95a-ec22-4310-bc77-a921581aa6c7.png)

<br/>
<br/>
<br/>
<br/>
<br/>

### ii)Write the image
![image](https://user-images.githubusercontent.com/70213227/161099503-2cf16a47-8935-4619-98d6-57841300e26f.png)
### iii)Shape of the Image

![image](https://user-images.githubusercontent.com/70213227/161100405-245c3a72-4395-4b31-9425-480c405f0c17.png)

<br/>
<br/>
<br/>
<br/>
<br/>

### iv)Access rows and columns
![image](https://user-images.githubusercontent.com/70213227/161100350-d0702856-57d1-480c-abc5-6ca6809d1ae6.png)

### v)Cut and paste portion of image

![image](https://user-images.githubusercontent.com/70213227/161100351-1c912020-454d-46fb-af24-4043c7c49943.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.
