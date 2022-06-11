# SA-C-GENDER-CLASSIFIER
# Algorithm
1.Install deepface

2.Import necessary packages

3.Read the image

4.Analyze the gender using deepface

## Program:
```python
/*
Program to implement Gender Classification
Developed by   : Gowri M
RegisterNumber :  212220230019
*/
#install deepface
pip install deepface

#import packages
from deepface import DeepFace
import cv2
import matplotlib.pyplot as plt

#read the image
img=cv2.imread('GowriM.jpeg')
plt.imshow(img[:,:,::-1])
plt.show()

#Analyze gender
result=DeepFace.analyze(img,actions=['gender'])
result2=DeepFace.analyze(img,actions=['emotion'])

#print the gender
print("Gender : ",result['gender'])
```

## OUTPUT:

1. CODE :

![Screenshot_717](https://user-images.githubusercontent.com/75235455/172542071-27da5290-1b11-47dd-858a-a8b410c703c1.png)

2. DEMO VIDEO YOUTUBE LINK:
</br>
#### Gender classification
</br>
   https://youtu.be/RSu7BteW7u4
