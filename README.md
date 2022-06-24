# working-on-image
## program:
```python

# Developed By:KUMARAN.B
# Register Number:212220230026

import cv2
import matplotlib.pyplot as plt
img=cv2.imread("kumaran b.jpg",1)
img=cv2.resize(img,(400,300))
plt.title('Flower(original image)')
plt.imshow(img)


# gray image
gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
plt.title('Gray Image')
plt.imshow(gray)


# hsv image
hsv = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
plt.title("Hsv Image")
plt.imshow(hsv)
h,s,v=cv2.split(hsv)

# h plane
plt.title('H plane')
plt.imshow(h)

# s plane
plt.title('S plane')
plt.imshow(s)

# v plane
plt.title('V plane')
plt.imshow(v)
```
## <br><br><br>Output
![Screenshot (370)](https://user-images.githubusercontent.com/75243072/175523485-af54af40-b714-424f-b684-8c619f87b817.png)

