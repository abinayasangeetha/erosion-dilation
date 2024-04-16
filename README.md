# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>Import the necessary packages


### Step2:
<br>Create the Text using cv2.putText

### Step3:
<br>Create the structuring element

### Step4:
<br>Erode the image

### Step5:
<br>Dilate the image

### Step6:
Display the output images
 
## Program:

# Import the necessary packages
```
import cv2
import numpy as np 
import matplotlib.pyplot as plt
```
# Create the Text using cv2.putText
```
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Abinaya',(5,70),font,2,(255),5,cv2.LINE_AA)
```

# Create the structuring element
```
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
```

# Erode the image
```
image_erode1=cv2.erode(img1,kernel1)
plt.imshow(image_erode1)
plt.axis("off")
```

# Dilate the image
```
image_dilate1=cv2.dilate(img1,kernel1)
plt.imshow(image_dilate1)
plt.axis("off")
```



## Output:

### Display the input Image
<br>
![image](https://github.com/abinayasangeetha/erosion-dilation/assets/119393675/9feae964-6d40-4e50-812a-df1af20bb39e)

<br>

### Display the Eroded Image
<br>
![image](https://github.com/abinayasangeetha/erosion-dilation/assets/119393675/643162fc-f0eb-4ca0-95ce-0d7d54fd0f08)

<br>

### Display the Dilated Image
<br>
![image](https://github.com/abinayasangeetha/erosion-dilation/assets/119393675/fe22f911-bcb5-4130-84ea-034c87da0b32)

<br>


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
