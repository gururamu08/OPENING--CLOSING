# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages
<br>


### Step2:
Read the image
<br>

### Step3:
Create the structuring element or kernal element
<br>

### Step4:
Use Opening operation
<br>

### Step5:
Use Closing Operation
<br>

 
## Program:

```
DEVELOPED BY:GURUMOORTHI R
REG NO: 212222230042
```

``` Python
# Import the necessary packages

import cv2
import numpy as np

# Create the Text using cv2.putText

img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_PLAIN
cv2.putText(img1,'GURUMOORTHI R',(5,35),font,2,(255),5,cv2.LINE_AA)
cv2.imshow("GURUMOORTHI R_212222230042",img1)
cv2.waitKey()
cv2.destroyAllwindows()



# Create the structuring element

kernal=np.ones((5,5),np.uint8)


# Use Opening operation

mg1o=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernal)
cv2.imshow("GURUMOORTHI R_212222230042",img1)
cv2.waitKey(0)
cv2.destroyAllwindows()


# Use Closing Operation

imglc=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernal)
cv2.imshow("GURUMOORTHI R_212222230042",imglc)
cv2.waitKey(0)
cv2.destroyAllwindows()



```
## Output:

### Display the input Image

![1](https://github.com/gururamu08/OPENING--CLOSING/assets/118707009/f1b4386b-443d-4277-bdc9-8f366864f3a0)



<br>

### Display the result of Opening

![2](https://github.com/gururamu08/OPENING--CLOSING/assets/118707009/69902ed8-2b62-4c39-8f50-b8a372e43315)



<br>

### Display the result of Closing

![3](https://github.com/gururamu08/OPENING--CLOSING/assets/118707009/ffe913f7-aa1a-4b65-9f97-4636ea0bed37)


<br>

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
