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
```
Jeswanth 212221230042
```
### Register Number: 
i) #To Read,display the image
```
import cv2
img = cv2.imread('ban.jpg', -1)
resized_img = cv2.resize(img, None, fx=0.5, fy=0.5, interpolation=cv2.INTER_LINEAR)
cv2.imshow('Jeswanth-212221230042', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
  

```
ii) #To write the image
```
import cv2
img=cv2.imread('ban.jpg',-1)
cv2.imwrite('ban.png',img)



```
iii) #Find the shape of the Image
```python3
import cv2
img=cv2.imread('ban.jpg',-1)
print(img.shape)



```
iv) #To access rows and columns

```python3
import cv2
img = cv2.imread('ban.jpg', -1)
resized_img = cv2.resize(img, None, fx=0.5, fy=0.5, interpolation=cv2.INTER_LINEAR)
for i in range(100,250):
for j in range(100,500):
    resized_img[i][j]=[255,250,255]
cv2.imshow('Jeswanth-212221230042',resized_img);
cv2.waitKey(0)
cv2.destroyAllWindows()



```
v) #To cut and paste portion of image
```python3
import cv2
img1=cv2.imread('ban.jpg',-1)
resized_img = cv2.resize(img, None, fx=0.5, fy=0.5, interpolation=cv2.INTER_LINEAR)
copied_portion=resized_img[150:250,250:450]
resized_img[350:450,550:750]=copied_portion
cv2.imshow('Jeswanth-212221230042',resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()



```

## Output:

### i) Read and display the image

<br>
<img width="324" alt="image" src="https://github.com/Jeswanth21001768/READ-AND-WRITE-IMAGE/assets/94155480/73570f06-4af0-4cfc-b10e-f96f0f79477b">

<br>

### ii)Write the image

<br>
<img width="738" alt="image" src="https://github.com/Jeswanth21001768/READ-AND-WRITE-IMAGE/assets/94155480/5613b3c2-65ff-4f17-9c20-2533de14635a">
<img width="328" alt="image" src="https://github.com/Jeswanth21001768/READ-AND-WRITE-IMAGE/assets/94155480/3ddbbafa-f846-4ecf-8252-02544c5a7657">


<br>

### iii)Shape of the Image

<br>
<img width="229" alt="image" src="https://github.com/Jeswanth21001768/READ-AND-WRITE-IMAGE/assets/94155480/24149942-b3a2-4c7a-9e7d-3d13ac8b043f">

<br>

### iv)Access rows and columns
<br>
<img width="753" alt="image" src="https://github.com/Jeswanth21001768/READ-AND-WRITE-IMAGE/assets/94155480/bbb33173-89ae-4f34-a924-b2fbc813a63d">


<br>

### v)Cut and paste portion of image
<br>
<img width="736" alt="image" src="https://github.com/Jeswanth21001768/READ-AND-WRITE-IMAGE/assets/94155480/8971e160-c7e9-477d-9ea6-1811b4bbdc07">

<br>

## Result:
Thus the images are read, displayed, and written successfully using the Python program.
