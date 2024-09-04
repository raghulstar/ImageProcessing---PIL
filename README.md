# 🖼️ Image Processing in Google Colab

This project showcases basic image processing techniques using Python's PIL (Pillow) library and Matplotlib within a Google Colab environment. The images are loaded directly from Google Drive, where various operations such as image multiplication, addition, inversion, rotation, and edge detection are performed.

## 🚀 Features

- **🔗 Mount Google Drive**: Seamlessly access and manipulate images stored in Google Drive.
- **📂 Load Images**: Easily load images into the Colab environment for processing.
- **🖼️ Display Images**: Visualize images side by side using Matplotlib.
- **⚙️ Image Operations**:
  - Multiply and add images
  - Convert images to greyscale
  - Invert images and perform image subtraction
  - Rotate images at specified angles
  - Apply Gaussian Blur for softening
  - Detect and highlight edges in images
  - Change edge colors for visual enhancement
- **💾 Save Processed Images**: Save your final processed images back to Google Drive with a single command.

## 🛠️ Getting Started

### Prerequisites

- A Google account with access to Google Drive.
- Basic knowledge of Python and image processing concepts.

### Running the Code

1. **Open in Colab**: Run the code directly in Google Colab. Ensure that the images (`x.png` and `o.png`) are uploaded to your Google Drive.

2. **Mount Google Drive**: Execute the following command to mount your Google Drive:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')

