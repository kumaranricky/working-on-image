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

hsv = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
plt.title("Hsv Image")
plt.imshow(hsv)
h,s,v=cv2.split(hsv)

plt.title('H plane')
plt.imshow(h)
plt.title('S plane')
plt.imshow(s)
plt.title('V plane')
plt.imshow(v)
