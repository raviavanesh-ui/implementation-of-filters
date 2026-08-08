# implementation-of-filters


# Implementation-of-filter
## Aim:
To implement filters for smoothing and sharpening the images in the spatial domain.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1
</br>
</br> 

### Step2
</br>
</br> 

### Step3
</br>
</br> 

### Step4
</br>
</br> 

### Step5
</br>
</br> 

## Program:
### Developed By   :Avanesh.R
### Register Number:212225240018
</br>

```

import cv2
import matplotlib.pyplot as plt
import numpy as np
image1=cv2.imread("TikTok - Make Your Day.jpg")
image2=cv2.cvtColor(image1,cv2.COLOR_BGR2RGB)
kernel=np.ones((11,11),np.float32)/169
image3=cv2.filter2D(image2,-1,kernel)
plt.figure(figsize=(9,9))
plt.subplot(1,2,1)
plt.imshow(image2)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(image3)
plt.title("Average Filter Image")
plt.axis("off")
plt.show()
kernel1=np.array([[1,2,1],[2,4,2],[1,2,1]])/16
image2=cv2.cvtColor(image1,cv2.COLOR_BGR2RGB)
image3=cv2.filter2D(image2,-1,kernel1)
plt.subplot(1,2,1)
plt.imshow(image2)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(image3)
plt.title("Weighted Average Filter Image")
plt.axis("off")
plt.show()
gaussian_blur=cv2.GaussianBlur(image2,(33,33),0,0)
plt.subplot(1,2,1)
plt.imshow(image2)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(gaussian_blur)
plt.title("Gaussian Blur")
plt.axis("off")
plt.show()
median=cv2.medianBlur(image2,13)
plt.figure(figsize=(9,9))
plt.subplot(1,2,1)
plt.imshow(image2)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(median)
plt.title("Median Blur")
plt.axis("off")
plt.show()
kernel2=np.array([[-1,-1,-1],[2,-2,1],[2,1,-1]])
image3=cv2.filter2D(image2,-1,kernel2)
plt.subplot(1,2,1)
plt.imshow(image2)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(image3)
plt.title("Laplacian Kernel")
plt.axis("off")
plt.show()
laplacian=cv2.Laplacian(image2,cv2.CV_64F)
plt.subplot(1,2,1)
plt.imshow(image2)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(laplacian)
plt.title("Laplacian Operator")
plt.axis("off")
plt.show()
```
<img width="717" height="219" alt="download" src="https://github.com/user-attachments/assets/e0a2257b-b38d-446e-96a0-47fbb4d44a5a" />

<img width="516" height="168" alt="download" src="https://github.com/user-attachments/assets/f3ff2c89-d23c-4a65-95f6-bd2f2e3cdf0b" />

<img width="717" height="219" alt="download" src="https://github.com/user-attachments/assets/a9c00c52-01a7-433d-a850-84a7fe443b08" />

<img width="516" height="168" alt="download" src="https://github.com/user-attachments/assets/8fc36df1-346f-4174-b428-669f32f3597b" />

<img width="717" height="219" alt="download" src="https://github.com/user-attachments/assets/8ef91d75-e1f6-4ebb-bd1d-b92c223f345c" />

<img width="533" height="168" alt="download" src="https://github.com/user-attachments/assets/13db3c60-a69a-4fee-b791-48ca1951b622" />








## Result:
Thus the filters are designed for smoothing and sharpening the images in the spatial domain.
