### Ex No: 10
### Date:

# <p align="center"> Implementation-of-Erosion-and-Dilation </p>

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
img2=cv2.putText(img1,"Srinivasan S",(5,70),font,3,(255),5,cv2.LINE_AA)
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
![image](https://user-images.githubusercontent.com/103049243/235292855-f15bed5a-dfe3-4d06-8899-16baa55bc183.png)

### Display the Eroded Image
![image](https://user-images.githubusercontent.com/103049243/235292894-d6cccc0f-fac4-4e33-858e-6382c050f26c.png)

### Display the Dilated Image
![image](https://user-images.githubusercontent.com/103049243/235293590-e8490bcc-a425-4ac6-848b-be037facd430.png)



## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
