# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
```
Step1:
Choose an image and save it as a filename.jpg

Step2:
Use imread(filename, flags) to read the file.

Step3:
Use imshow(window_name, image) to display the image.

Step4:
Use imwrite(filename, image) to write the image.

Step5:
End the program and close the output image windows.
```

## Program:
### Developed By:G.Jayanth
### Register Number:212221230030 
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('1.jpg',1)
cv2.imshow('212221230030 jayanth',color_img)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
color_img=cv2.imread('1.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212221230030 jayanth',color_img)
cv2.waitKey(0) 


```
iii) #Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('1.jpg',1)
print(color_img.shape)
```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('1.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221230030 jayanth',color_img)
cv2.waitKey(0)
```
v) #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('1.jpg',-1)
tag=color_image[30:40,30:40]
color_image[5:15,5:15]=tag
cv2.imshow('212221230030 jayanth',color_image)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

<img width="209" alt="Read and display the image" src="https://github.com/JayanthYadav123/READ-AND-WRITE-IMAGE/assets/94836154/1aba7a91-8171-4422-8b50-46c6a16412f6">


### ii)Write the image

<img width="227" alt="write the image" src="https://github.com/JayanthYadav123/READ-AND-WRITE-IMAGE/assets/94836154/8b7aa8d0-3e90-4a42-b845-ddad22c7fe37">


### iii)Shape of the Image

<img width="408" alt="image" src="https://github.com/JayanthYadav123/READ-AND-WRITE-IMAGE/assets/94836154/db027aae-9652-4cf3-b964-069f428ca594">


### iv)Access rows and columns
<img width="209" alt="ACESSING ROW AND COLUMN" src="https://github.com/JayanthYadav123/READ-AND-WRITE-IMAGE/assets/94836154/97657437-8858-4926-9099-8014961e1e29">


### v)Cut and paste portion of image
<img width="208" alt="Cut and paste portion of image" src="https://github.com/JayanthYadav123/READ-AND-WRITE-IMAGE/assets/94836154/c33c797e-7986-41c1-9d2b-4511cd59df61">

## Result:
Thus the images are read, displayed, and written successfully using the python program.
