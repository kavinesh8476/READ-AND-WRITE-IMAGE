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
### Developed By:Kavinesh M
### Register Number: 212222230064
i) #To Read,display the image
```python3
import cv2
img = cv2.imread('d.jpg', 1)
cv2.imshow('212222240064_Kavinesh', img)
cv2.waitKey(0)
```
ii) #To write the image
```python3
import cv2
img = cv2.imread('d.jpg', 1)
new_img = cv2.imwrite('d_c.jpg', img)
cv2.imshow('212222240064_Kavinesh', img)
cv2.waitKey(0)
```
iii) #Find the shape of the Image
```python3
import cv2
img = cv2.imread('d.jpg', 1)
print(img.shape)
```
iv) #To access rows and columns

```python3
import cv2
import random
img = cv2.imread('d.jpg', 1)
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)]
cv2.imshow('part image', img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
v) #To cut and paste portion of image
```python3
import cv2
img = cv2.imread('d.jpg', 1)
tag = img[300:400, 300:400]
img[50:150, 50:150] = tag
cv2.imshow('212222240064_Kavinesh', img)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image
![readanddis](https://github.com/kavinesh8476/READ-AND-WRITE-IMAGE/assets/118466561/08671beb-14d4-419b-b0cc-309ca991a4df)

<br>
<br>

### ii)Write the image
![write](https://github.com/kavinesh8476/READ-AND-WRITE-IMAGE/assets/118466561/f74f97c9-aa20-4a07-adbb-ed044888d9dd)

<br>
<br>

### iii)Shape of the Image
![shape](https://github.com/kavinesh8476/READ-AND-WRITE-IMAGE/assets/118466561/df19fc25-6d2e-4871-977d-eef217a3ba4a)

<br>
<br>

### iv)Access rows and columns

![rowsand columns](https://github.com/kavinesh8476/READ-AND-WRITE-IMAGE/assets/118466561/e2c6af8d-6993-4268-8072-39ef76719488)
<br>
<br>

### v)Cut and paste portion of image
![cutandpaste](https://github.com/kavinesh8476/READ-AND-WRITE-IMAGE/assets/118466561/14dd6ced-6303-4997-8eda-874ac861e7d6)

<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
