# DICOM Workflow Automation README

This project comprises a series of Jupyter Notebooks designed to automate the workflow for processing DICOM medical imaging files. The process includes analysis, PDF embedding, and media conversion, aiming to simplify and streamline the handling of DICOM files.

## Contents

- `analysis.ipynb`: Manages initial DICOM file processing, including image conversion and metadata extraction.
- `embedPDF.ipynb`: Handles the conversion of images into a PDF layout and merges this PDF with another document.
- `media.ipynb`: Converts a set of images into a video and then a GIF for easy dissemination and review.

## Requirements

- Python 3.11.4
- Jupyter Notebook or JupyterLab
- Required Python Libraries:
  - `pydicom` for DICOM file reading.
  - `PIL` (Python Imaging Library) for image operations.
  - `pytesseract` for OCR capabilities (optional).
  - `reportlab` for PDF creation.
  - `PyPDF2` for PDF manipulation.
  - `cv2` (OpenCV) for video processing.
  - `moviepy` for video to GIF conversion.

## Setup Instructions

1. Ensure Python 3.x is installed.
2. Install necessary libraries using: `pip install pydicom pillow pytesseract reportlab PyPDF2 opencv-python moviepy`
3. Clone this repository or download the notebooks.
4. Open the notebooks in JupyterLab or Jupyter Notebook.

## Usage Guide

### analysis.ipynb

Converts DICOM files to images and extracts metadata.

1. Define `dicom_folder` and `output_folder` for DICOM files and image output.
2. Execute the notebook to process DICOM files into PNG images and extract metadata.

### embedPDF.ipynb

Converts images into a PDF and appends it to another PDF.

1. Set `image_folder_path`, `images_pdf_path`, `main_pdf_path`, and `final_pdf_path`.
2. Run the notebook to create a PDF from images and merge it with an existing PDF document.

### media.ipynb

Converts images into a video and then into a GIF.

1. Specify `pathIn` for image source and `pathOut` for video output.
2. Define `video_path` for video input and `gif_path` for GIF output.
3. Run the notebook to generate a video and convert it into a GIF.

