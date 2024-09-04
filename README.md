🖼️ Image Processing in Google Colab
This project showcases basic image processing techniques using Python's PIL (Pillow) library and Matplotlib within a Google Colab environment. The images are loaded directly from Google Drive, where various operations such as image multiplication, addition, inversion, rotation, and edge detection are performed.
🚀 Features
🔗 Mount Google Drive: Seamlessly access and manipulate images stored in Google Drive.
📂 Load Images: Easily load images into the Colab environment for processing.
🖼️ Display Images: Visualize images side by side using Matplotlib.
⚙️ Image Operations:
  - Multiply and add images
  - Convert images to greyscale
  - Invert images and perform image subtraction
  - Rotate images at specified angles
  - Apply Gaussian Blur for softening
  - Detect and highlight edges in images
  - Change edge colors for visual enhancement

💾 Save Processed Images: Save your final processed images back to Google Drive with a single command.

🛠️ Getting Started
Prerequisites
- A Google account with access to Google Drive.
- Basic knowledge of Python and image processing concepts.
Running the Code
1. **Open in Colab**: Run the code directly in Google Colab. Ensure that the images (`x.png` and `o.png`) are uploaded to your Google Drive.
2. **Mount Google Drive**: Execute the following command to mount your Google Drive:
3. **Load and Process Images**: Load images using their respective paths from Google Drive, then perform the image processing operations as outlined in the code.
4. **Save the Processed Image**: Save the final processed image back to Google Drive as `processed.png`.

from google.colab import drive
drive.mount('/content/drive')
📝 Code Example
from PIL import Image, ImageChops, ImageFilter
from matplotlib import pyplot as plt

# Mounting Google Drive
from google.colab import drive
drive.mount('/content/drive')

# Loading images from Drive
image_x = "/content/drive/My Drive/x.png"
image_o = "/content/drive/My Drive/o.png"

# Creating PIL image objects
x = Image.open(image_x)
o = Image.open(image_o)

# Displaying images side by side
plt.subplot(121), plt.imshow(x)
plt.axis('off')
plt.subplot(122), plt.imshow(o)
plt.axis('off')

# Image processing operations (multiply, add, greyscale, invert, etc.)
...

# Saving the final processed image
edge.save('/content/drive/My Drive/processed.png')
📊 Output
The code generates several processed images, including:
- **Greyscale Image**: Converts the original image to greyscale.
- **Inverted Image**: Inverts the colors of the image.
- **Rotated Image**: Rotates the image by 45 degrees.
- **Blurred and Edge Detected Image**: Applies Gaussian blur and detects edges.
- **Filled Edge Image**: Enhances edge visibility with color changes.
📄 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
🙌 Acknowledgments
- **[Google Colab](https://colab.research.google.com)**: For providing a robust platform to run Python code in the cloud.
- **[Pillow (PIL)](https://python-pillow.org/)**: For powerful and easy-to-use image processing capabilities.
