# Image to PDF Converter

## Introduction

This is a simple desktop application built with Python that allows users to convert multiple images into a single PDF file. The application provides a graphical user interface (GUI) for selecting images, specifying the output PDF name, and performing the conversion. Each selected image is placed on a separate page in the PDF, scaled to fit within the page dimensions and centered.

## Tech Stack

- **Python**: The core programming language used for the application.
- **Tkinter**: A standard Python library for creating graphical user interfaces (GUIs). It provides the window, buttons, labels, and listbox for user interaction.
- **Pillow (PIL)**: A Python imaging library used to open, manipulate, and handle image files (supports PNG, JPG, JPEG formats).
- **ReportLab**: A library for generating PDF documents programmatically. It is used to create the PDF canvas, draw images onto pages, and save the final PDF file.

## Prerequisites

Before running the application, ensure you have Python installed on your system (version 3.6 or higher is recommended). You also need to install the required dependencies:

1. Install Pillow: `pip install pillow`
2. Install ReportLab: `pip install reportlab`

You can install both at once with: `pip install pillow reportlab`

## How to Run the Code

1. Clone or download the project files to your local machine.
2. Open a terminal or command prompt and navigate to the project directory (e.g., `cd path/to/image-converter`).
3. Run the application using Python: `python app.py`
4. The GUI window will open, allowing you to interact with the application.

## Usage

1. **Upload Images**: Click the "Upload Images" button to open a file dialog. Select one or more image files (PNG, JPG, JPEG). The selected images will be listed in the listbox below the button.
2. **Enter Output PDF Name**: In the text field labeled "Enter output PDF name:", type the desired name for the output PDF file (without the .pdf extension). If left blank, the default name "output.pdf" will be used.
3. **Convert to PDF**: Click the "Convert to PDF" button to start the conversion process. The application will create a PDF file with each image on a separate page, scaled and centered.
4. The PDF file will be saved in the same directory as the application.

## Output

The application generates a PDF file containing all selected images. Each image is:
- Scaled to fit within the page dimensions (540x720 points, leaving margins).
- Centered on the page.
- Placed on a white background.

The output PDF file will be named as specified (or "output.pdf" by default) and saved in the current working directory. This demonstrates that the images have been successfully converted into a PDF document by the code.

## Notes

- Supported image formats: PNG, JPG, JPEG.
- The PDF page size is fixed at 8.5x11 inches (612x792 points).
- If no images are selected, the conversion will not proceed.
- Ensure that the output PDF name does not conflict with existing files in the directory.