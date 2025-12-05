# laplacian-image-sharpening
Laplacian-based image sharpening and edge detection implemented with OpenCV.

---

## Project Overview

This repository contains:

- A Python script that:
  - Loads a grayscale Moon image
  - Applies a Laplacian convolution kernel
  - Generates a Laplacian output image
  - Combines the Laplacian with the original to create a sharpened result
  - Displays all images using Matplotlib

---

## How the Algorithm Works

1. **Load the image**  
   The Moon image is loaded in grayscale using OpenCV.

2. **Define Laplacian Kernel**  
   A custom 3×3 Laplacian kernel is used to detect edges and high‑frequency details.

3. **Apply the Laplacian Filter**  
   Convolution is performed using `cv2.filter2D`.

4. **Sharpen the Image**  
   The Laplacian output is added back to the original image using `cv2.addWeighted`.

5. **Visualization**  
   The script displays:
   - Original Image  
   - Laplacian Output  
   - Sharpened Image  
   - A combined 3‑panel comparison

---

## Example Outputs

Below are placeholders where your images should appear:

### Original Moon Image  
<img width="419" height="504" alt="image" src="https://github.com/user-attachments/assets/aeda6248-8570-47ac-9e55-c567f510a376" />

### Laplacian Filter Result  
<img width="419" height="504" alt="image" src="https://github.com/user-attachments/assets/59b886fb-cd8d-4959-9e20-cea0b4de2f5c" />

### Sharpened Image (Original + Laplacian)  
<img width="419" height="504" alt="image" src="https://github.com/user-attachments/assets/93e81832-b6ae-46f3-b0e9-f5fc7a7d8019" />

### Three‑Panel Comparison  
<img width="1173" height="427" alt="image" src="https://github.com/user-attachments/assets/ae807dd4-ec86-42c9-8130-d61feea96262" />

---

## laplacian_kernel
```
[-1, -1, -1]
[-1,  8, -1]
[-1, -1, -1]
```
---
