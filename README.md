# SA-C-GENDER-CLASSIFIER
# Algorithm
1. Install the DeepFace library using the command pip install deepface
2. To Predict the gender of a person use this DeepFace library
3. Import the deepface class from DeepFace library, cv2 class from openCv2 library and Matplot library according to the requirements.
4. Load and display the image which we have imported. 
5. Pass the image to DeepFace library and analyze the image to predict gender of a person.
6. This prediction is stored in result variable and print the prediction using this algorithm.

## Program:
```
/*
Program to implement 
Developed by   : Dineshkumar S
RegisterNumber :  212220230012
*/
```

```
from deepface import DeepFace
import cv2
import matplotlib.pyplot as plt
img1=cv2.imread('img2.webp')
plt.imshow(img1[:,:,::-1])
plt.axis("off")
plt.show()
result=DeepFace.analyze(img1,actions=['gender'])
print("Gender : ",result['gender'])
img2=cv2.imread('img1.webp')
plt.imshow(img2[:,:,::-1])
plt.axis("off")
plt.show()
result=DeepFace.analyze(img2,actions=['gender'])
print("Gender : ",result['gender'])
```

## OUTPUT:
![Screenshot (231)](https://user-images.githubusercontent.com/75234807/173243409-ba504e95-925e-422e-9a5a-a0e9a969f21b.png)

DEMO VIDEO YOUTUBE LINK:
