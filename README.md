# Clone Catch
## Image Duplicate Detection and Face Recognition

This project implements an image duplicate detection system along with a face recognition feature. It identifies and processes images in a specified folder, converting them to JPEG format if necessary, detecting duplicates, and moving images containing specified faces to designated folders.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Features

- Convert images from HEIC and other formats to JPEG.
- Detect and move duplicate images to a dedicated folder.
- Extract face encodings using the VGG16 model for image features.
- Search for and organize images based on face recognition from reference images.
- Move matching images to a folder named after the identified person.

## Requirements

- Python 3.x
- Libraries:
  - `numpy`
  - `Pillow`
  - `pillow-heif`
  - `Keras`
  - `face_recognition`
  - `opencv-python`
  
You can install the required libraries using pip:

```bash
pip install numpy Pillow pillow-heif keras face_recognition opencv-python
```
## Installation
1. Clone the repository:
```bash
git clone <repository-url>
```

2. Navigate to the project directory:
```bash
cd <project-directory>
```
3. Install the required libraries as mentioned above.

## Usage
1. Place all images in the ./images/ folder.
2. Run the conversion script to convert images to JPEG and organize videos:

```python
python convert_images.py
```
3. To identify duplicate images and move them to the dupes and best folders, run:
```python
python identify_duplicates.py
```

4. To move matching images based on a reference image, run:
```python
python move_matching_images.py
```
Input the filenames of the reference images and the person's name when prompted.

