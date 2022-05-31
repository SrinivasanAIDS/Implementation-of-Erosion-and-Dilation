# Implementation-of-Erosion-and-Dilation

## Aim
To implement Erosion and Dilation using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step1:
Import the necessary packages.
<br>

### Step2:
Create the Text using cv2.putText
<br>

### Step3:
Create the structuring element.
<br>

### Step4:
Erode the image.
<br>

### Step5:
Dilate the image.
<br>

 
## Program:

``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1=np.zeros((300,500),dtype='uint8')
font=cv2.FONT_ITALIC=3
img2=cv2.putText(img1,"Kumar",(5,70),font,3,(255),5,cv2.LINE_AA)
cv2.imshow("Original",img2)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Create the structuring element
kernel1=np.ones((5,5),np.uint8)

# Erode the image
erode=cv2.erode(img2,kernel1)
cv2.imshow("Erosion1",erode)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Dilate the image
dilute=cv2.dilate(img2,kernel2)
cv2.imshow("Dilution",dilute)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
## Output:

### Display the input Image
![image](https://user-images.githubusercontent.com/103049243/171180516-a1f8da63-d16f-4da6-b068-bc3760bd14b6.png)

### Display the Eroded Image
![image](https://user-images.githubusercontent.com/103049243/171180677-af1d1945-1bbc-42e5-8c9a-5302011656c5.png)

### Display the Dilated Image
![image](https://user-images.githubusercontent.com/103049243/171180788-a89b3cf2-92cb-4435-aa81-35a90eae2e2e.png)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
