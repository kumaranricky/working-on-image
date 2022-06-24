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
![Screenshot (371)](https://user-images.githubusercontent.com/75243072/175524229-4143ff6a-0867-4133-9e8f-66d220d88acf.png)


