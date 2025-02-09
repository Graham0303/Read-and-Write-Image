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

# Developed By: Graham Stanes A
# Register Number: 212220230020

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
![Screenshot (6)](https://user-images.githubusercontent.com/75235488/160637901-41bf4705-0fa6-4d32-a1ab-71e4b7c1c774.png)

![Screenshot (7)](https://user-images.githubusercontent.com/75235488/160637970-e3c1659a-f887-49c3-b7e5-b9850f81e8b2.png)

<br/>
<br/>
<br/>
<br/>
<br/>

### ii)Write the image
![Screenshot (8)](https://user-images.githubusercontent.com/75235488/160638028-5e4fc52c-ad38-4694-a9c3-04043ae14617.png)
### iii)Shape of the Image

![Screenshot (11)](https://user-images.githubusercontent.com/75235488/160641197-e200baae-3551-45c7-93f0-6921505f957e.png)

<br/>
<br/>
<br/>
<br/>
<br/>

### iv)Access rows and columns
![Screenshot (9)](https://user-images.githubusercontent.com/75235488/160638115-4acf9beb-7255-42c9-a143-727854cb645f.png)

### v)Cut and paste portion of image

![Screenshot (24)](https://user-images.githubusercontent.com/75235488/161490446-327dd538-6a14-41a0-820b-71a8bf098afa.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.

