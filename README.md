
# Image Processing Tool

This project provides a set of tools for image processing, including cropping images and removing backgrounds. It includes a Streamlit web application for easy interaction with the processing functions.

## Contents

1. [Main Application (app.py)](#main-application-apppy)
2. [Streamlit Web Interface (streamlit_app.py)](#streamlit-web-interface-streamlit_apppy)
3. [Dependencies (requirements.txt)](#dependencies-requirementstxt)
4. [Version Control (.gitignore and .gitattributes)](#version-control-gitignore-and-gitattributes)

## Main Application (app.py)

### Functions

#### `crop_images_in_folder(folder_path, output_size=(224, 224))`

This function processes all images in a specified folder, cropping them to a given size.

**Inputs:**
- `folder_path` (str): Path to the folder containing images
- `output_size` (tuple): Desired output size (width, height), default is (224, 224)

**Outputs:**
- Cropped images saved in a subdirectory named 'cropped_images'

#### `remove_background(input_folder, output_folder)`

This function removes the background from all images in a specified folder.

**Inputs:**
- `input_folder` (str): Path to the folder containing images
- `output_folder` (str): Path where processed images will be saved

**Outputs:**
- Images with removed backgrounds saved in the specified output folder

## Streamlit Web Interface (streamlit_app.py)

This file creates a user-friendly web interface using Streamlit, allowing users to interact with the image processing functions.

**Features:**
- Input field for specifying the image folder path
- Buttons to trigger image cropping and background removal operations
- Success messages upon completion of operations

## Dependencies (requirements.txt)

The project requires the following Python packages:
- streamlit
- Pillow
- rembg

## Version Control (.gitignore and .gitattributes)

- `.gitignore`: Specifies files and directories that should be ignored by Git version control
- `.gitattributes`: Configures Git to use LF (Line Feed) normalization for text files

## Usage

1. Install the required dependencies using `pip install -r requirements.txt`
2. Run the Streamlit app using `streamlit run streamlit_app.py`
3. Enter the path to your image folder in the web interface
4. Use the provided buttons to crop images or remove backgrounds

This tool is designed for easy batch processing of images, particularly useful for preparing datasets for machine learning models or cleaning up image collections.
