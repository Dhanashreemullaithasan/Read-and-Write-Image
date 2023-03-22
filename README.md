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
### Developed By:DHANASHREE M
### Register Number: 212221230018
i) #To Read,display the image
```
import cv2
N=cv2.imread("flower.jpg",1)
cv2.imshow("new",N)
cv2.waitKey(0)  

```
ii) #To write the image
```
import cv2
N=cv2.imread("flower.jpg",1)
cv2.imwrite("flower.jpg",N)
cv2.imshow("new",N)
cv2.waitKey(0)
```
iii) #Find the shape of the Image
```
import random
import cv2
N=cv2.imread("flower.jpg",1)
for i in range(100):
    for j in range(N.shape[1]):
        N[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("new",N)
cv2.waitKey(0)
```
iv) #To access rows and columns

```
import random
import cv2
N=cv2.imread("flower.jpg",1)
for i in range(100):
    for j in range(N.shape[1]):
        N[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("new",N)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
N=cv2.imread("flower.jpg",1)
tag=N[140:240,165:180]
N[25:125,50:65]=tag
cv2.imshow("new",N)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

![output](./dip%20ex1.png)

### ii)Write the image

![output](./dipex12.png)

### iii)Shape of the Image

![output](./dipex13.png)

### iv)Access rows and columns
![output](./dipex14.png)

### v)Cut and paste portion of image
![output](./dipex15.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


