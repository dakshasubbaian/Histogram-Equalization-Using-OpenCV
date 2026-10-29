# Histogram Equalization Using OpenCV (Grayscale & Color Images)

---

## AIM:

To write a Python program using OpenCV to perform histogram equalization on both grayscale and color images to enhance image contrast and brightness.

The program performs the following operations:

- Read and display a grayscale image  
- Plot histogram of the grayscale image  
- Apply histogram equalization on grayscale image  
- Read and display a color image  
- Plot histogram of B, G, R channels  
- Convert image to HSV color space  
- Apply histogram equalization on the Value (V) channel  
- Convert the enhanced image back to BGR format  
- Display original and enhanced images with histograms  

---

## SOFTWARE USED:

- Anaconda – Python 3.7  
- Jupyter Notebook / VS Code  
- OpenCV (`cv2`)  
- NumPy  
- Matplotlib  

---

## Algorithm

### Step 1:
Import the required libraries: OpenCV, NumPy, and Matplotlib.

### Step 2:
Read the image `parrot.jpg` in grayscale format.

### Step 3:
Display the grayscale image and plot its histogram.

### Step 4:
Apply histogram equalization using `cv2.equalizeHist()` to enhance contrast.

### Step 5:
Display original grayscale image, its histogram, enhanced image, and its histogram using a 2 × 2 grid.

### Step 6:
Read the same image in color format.

### Step 7:
Split the image into B, G, R channels and plot their histograms.

### Step 8:
Convert the image from BGR to HSV color space.

### Step 9:
Apply histogram equalization on the V (Value) channel.

### Step 10:
Merge the channels and convert the image back to BGR format.

### Step 11:
Display original color image, histogram, enhanced image, and enhanced histogram using a 2 × 2 grid.

---

## Program

### Developed By:
**Name:** DAKSHA SUBBAIAN 

**Register No:** 212223230036

---
## PROGRAM:
### Display Grayscale Image
```
import cv2
import matplotlib.pyplot as plt

img_grayscale = cv2.imread("peacock.jpg", cv2.IMREAD_GRAYSCALE)

plt.imshow(img_grayscale, cmap="gray")
plt.title("Grayscale Image")
plt.show()
```

### Display Color Channels
```
img = cv2.imread("peacock.jpg")

B, G, R = cv2.split(img)

plt.figure(figsize=(12, 4))

plt.subplot(131)
plt.imshow(B, cmap="gray")
plt.title("Blue Channel")

plt.subplot(132)
plt.imshow(G, cmap="gray")
plt.title("Green Channel")

plt.subplot(133)
plt.imshow(R, cmap="gray")
plt.title("Red Channel")

plt.tight_layout()
plt.show()
```
##  OUTPUT:

### Grayscale Histogram Equalization
<img width="1227" height="835" alt="image" src="https://github.com/user-attachments/assets/22b16dee-48d0-4767-89e4-1cfe1a72aa2e" />
 

### Color Image Histogram Equalization
<img width="1227" height="848" alt="image" src="https://github.com/user-attachments/assets/75e6a906-3e06-4d93-9d10-271e89691198" />


---

## Result

Thus, histogram equalization is successfully performed on both grayscale and color images using OpenCV. The contrast and brightness of the images are significantly improved, enhancing visual quality and feature visibility.
