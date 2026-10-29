# Experiment 1:  Image-Handling-and-pixel-Transformation-Using-OpenCV-Asssignment

## Name: Sanchita Sandeep
## Register Number: 212224240142<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/7e156d66-1790-4bab-b480-9fdd88b5370b" />

---
## AIM
To perform image handling and pixel transformations using Python and OpenCV, including reading and displaying images, drawing shapes, adding text, color space conversion, pixel manipulation, image resizing, cropping, flipping, and saving the modified image.
## INSTALLATION

Install the required libraries using the following command:

```bash
pip install opencv-contrib-python-headless matplotlib
```
## ALGORITHM

### Step 1: Read and Display an Image

1. Import OpenCV and Matplotlib libraries.
2. Read an image from the local directory using `cv2.imread()`.
3. Convert the image from BGR to RGB.
4. Display the original image using Matplotlib.

### Step 2: Draw Shapes and Add Text

1. Draw a line from the top-left to the bottom-right of the image.
2. Draw a circle at the center of the image.
3. Draw a rectangle around the image.
4. Add the text "OpenCV Drawing" at the top-left corner.

### Step 3: Color Space Conversion

1. Convert the RGB image to HSV and display it.
2. Convert the RGB image to grayscale and display it.
3. Convert the RGB image to YCrCb and display it.
4. Convert the HSV image back to RGB and display it.

### Step 4: Pixel Manipulation

1. Access and print the pixel value at coordinates `(100, 100)`.
2. Change the pixel at coordinates `(200, 200)` to white.
3. Modify a 300 × 300 region of the image to white.
4. Display the modified image.

### Step 5: Image Resizing

1. Read the original image.
2. Resize the image to half its original width and height.
3. Display the resized image.
### Step 6: Image Cropping
1. Read the original image.
image = cv2.imread('riki.jpeg')

image.shape

# Crop a 300x300 region starting from (50, 50)
roi = image[50:350, 50:350]  # Rows: 50-349, Columns: 50-349

# Convert BGR to RGB for displaying with Matplotlib
roi_rgb = cv2.cvtColor(roi, cv2.COLOR_BGR2RGB)

# Display the cropped region (ROI)
plt.imshow(roi_rgb)
plt.title("Cropped Region of Interest (ROI)")
plt.axis("off")
plt.show()
```

### Step 7: Image Flipping

```python
# Load the image
image = cv2.imread('riki.jpeg')

# Flip the image horizontally (left-right)
flipped_horizontally = cv2.flip(image, 1)

# Convert BGR to RGB for displaying with Matplotlib
flipped_horizontally_rgb = cv2.cvtColor(flipped_horizontally, cv2.COLOR_BGR2RGB)

# Horizontal flip
plt.imshow(flipped_horizontally_rgb)
plt.title("Flipped Horizontally")
plt.axis("off")

# Flip the image vertically (up-down)
flipped_vertically = cv2.flip(image, 0)

# Convert BGR to RGB for displaying with Matplotlib
flipped_vertically_rgb = cv2.cvtColor(flipped_vertically, cv2.COLOR_BGR2RGB)

# Vertical flip
plt.imshow(flipped_vertically_rgb)
plt.title("Flipped Vertically")
plt.axis("off")
```

---
## OUTPUT

#The following outputs are obtained:

#1. Original image displayed using OpenCV and Matplotlib.

<img width="276" height="275" alt="Screenshot 2026-10-29 090059" src="https://github.com/user-attachments/assets/8b193a71-dd94-4f02-8744-edea6c9b8f2b" />

#2. Image with a line drawn from the top-left to the bottom-right.


<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/cec59a6d-5a3f-47fc-8321-2d6338536cfd" />



#3. Image with a circle .

<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/7be6771c-060a-4ce1-a312-b9691feb360f" />


#4. Image with a rectangle around its boundary.
<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/73e1909a-7b59-45fa-9b57-6ee9670666fe" />




#5. Image with the text "OpenCV drawing"

<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/3cd0defa-2adc-40e5-9ce4-fa7eb374cfa8" />




#6. HSV, grayscale, and YCrCb color space conversions.

#HSV conversion

<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/812c6ebc-a209-4594-9086-bf876f4f5820" />


#grayscale conversion

<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/abf0cbac-8d1d-4e16-832c-065adfe7c6b9" />


#YCrCb conversion

<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/ef3dd470-7660-449f-8bf5-7b2cfb635544" />


#7. Image converted from HSV back to RGB.

<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/1f43a04e-6b8a-47dd-ad2b-b61f8b0ffa39" />






#8. Pixel value displayed and a white region added to the image.
<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/67028982-f39d-46cd-b65e-f323f247c26d" />


#9. Image resized to half its original dimensions.
<img width="493" height="410" alt="download" src="https://github.com/user-attachments/assets/0a2ed9fe-7b5c-435b-a110-ddc4e6b96724" />



#10. Cropped region of interest displayed.


<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/40bf3bd0-a11c-42e9-bee0-487fc9e9bf55" />





#11. Horizontally flipped image displayed.
<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/e0b36a2b-99c8-43fe-b85b-b0a22003e3c6" />





#12. Vertically flipped image displayed.

<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/5026941a-719f-45fc-92ef-d549cd8508cf" />




## RESULT

Thus, image handling and pixel transformations were performed using Python, OpenCV, and Matplotlib. The experiment demonstrated image reading, shape drawing, text insertion, color space conversion, pixel manipulation, image resizing, cropping, flipping, and saving.

---

