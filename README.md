
# Experiment 1:  Image-Handling-and-pixel-Transformation-Using-OpenCV-Asssignment

## Name: Sanchita Sandeep
## Register Number: 212224240142
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

# 1. Original image displayed using OpenCV and Matplotlib.

<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/58a1073c-a708-4323-a1f7-eb676f5c3c46" />


# 2. Image with a line drawn from the top-left to the bottom-right.


<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/898b0d96-cb72-4cee-81b0-b4fbb9a6bb01" />

# 3. Image with a circle .

<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/45c8a720-8411-415f-be48-52fc8dd0c9bf" />

# 4. Image with a rectangle around its boundary.
<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/06458623-396f-49d9-8b8d-9d5b34b75b9a" />

# 5. Image with the text "OpenCV drawing"

<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/cafef7ec-feda-4ec0-b3f4-7e4a56e1409d" />


# 6. HSV, grayscale, and YCrCb color space conversions.

# HSV conversion

<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/85866074-0786-453b-a2f4-0c699ec0c2e1" />


# grayscale conversion

<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/9a1a1773-df0f-430e-8370-a40238080e1b" />


# YCrCb conversion

<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/99379494-5bd7-4ced-8437-b469f314f2c9" />


# 7. Image converted from HSV back to RGB.

<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/4fd011c0-6bd3-429f-b9f2-a3ac54582939" />


# 8. Pixel value displayed and a white region added to the image.
<img width="302" height="410" alt="download" src="https://github.com/user-attachments/assets/0ad89457-4093-4ee8-8818-95fd676f5d76" />


# 9. Image resized to half its original dimensions.
<img width="493" height="410" alt="download" src="https://github.com/user-attachments/assets/1e0c42f4-b30b-4e53-818d-0590927982cc" />

# 10. Cropped region of interest displayed.


<img width="389" height="410" alt="download" src="https://github.com/user-attachments/assets/0cbb8bf6-6c72-4cd2-a3fc-587a420e955c" />


# 11. Horizontally flipped image displayed.
<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/10d2480e-0cf3-4bb5-b997-3ca37b969e72" />


# 12. Vertically flipped image displayed.

<img width="297" height="410" alt="download" src="https://github.com/user-attachments/assets/794edab7-f6f7-4d27-ad0e-4390f07051ab" />


## RESULT

Thus, image handling and pixel transformations were performed using Python, OpenCV, and Matplotlib. The experiment demonstrated image reading, shape drawing, text insertion, color space conversion, pixel manipulation, image resizing, cropping, flipping, and saving.
