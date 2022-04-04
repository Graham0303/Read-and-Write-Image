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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
  import cv2
image_1=cv2.imread("pic_1.PNG")
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)

```
ii) #To write the image
```

cv2.imwrite("pic_1",image_1)


```
iii) #Find the shape of the Image
``python3

print(image_1.shape)


```
iv) #To access rows and columns
```python3

for i in range(70,90):
    for j in range(110,170):
        image_1[i][j]=[0,0,0]
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```python3

image_1[70:90,110:175]=image_1[70:90,110:175]
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image


![Screenshot (2)](https://user-images.githubusercontent.com/75235150/161493032-becb0f0f-f649-4b18-80c2-cc82e0625741.png)



### ii)Write the image


![Screenshot (2)](https://user-images.githubusercontent.com/75235150/161493042-5f3b9156-983c-47c5-9b52-6bd0b87c4f82.png)



### iii)Shape of the Image

![Screenshot (3)](https://user-images.githubusercontent.com/75235150/161493073-86a79e97-a6eb-4618-a089-4ca4d06a537a.png)



### iv)Access rows and columns

![Screenshot (4)](https://user-images.githubusercontent.com/75235150/161493103-fb663000-67fb-46b7-b119-2f76b9cbaaa3.png)



### v)Cut and paste portion of image
![Screenshot (5)](https://user-images.githubusercontent.com/75235150/161493131-ab4fa0f1-b705-487a-9f83-d393d1d54ac5.png)



## Result:
Thus the images are read, displayed, and written successfully using the python program.


