
# WORK SHOP-03: CANNY EDGE DETECTION
### Name: M.Mounika
### Register no: 212224040202

# AIM:
To perform Canny Edge Detection model through your laptop.

# PROGRAM:
```
import cv2
import matplotlib.pyplot as plt
```
```
img = cv2.imread('myphoto.jpg',cv2.IMREAD_GRAYSCALE)
```
```
blurred =cv2.GaussianBlur(img, (5,5),0)
```
```
edges = cv2.Canny(blurred, 50, 150)
```
```
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```
# OUTPUT:
<img width="957" height="538" alt="Screenshot 2025-10-14 233227" src="https://github.com/user-attachments/assets/7be39a5e-c3f4-4ce3-98a5-284bd3c7c28f" />

