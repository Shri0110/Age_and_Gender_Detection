# Age_and_Gender_Detection
https://drive.google.com/drive/folders/1nK6Y7jcCTugP6xRmOsrbMk091nQj-L89?usp=drive_link

All files available at^^

This repository contains Python code for detecting and estimating the age and gender of faces in images or videos using OpenCV and pre-trained deep learning model(Caffe model). The code uses a Convolutional Neural Network (CNN) to detect faces and then predicts the age and gender of the detected faces.

## Prerequisites

Before using this code, you'll need to have the following dependencies installed:

- Python (3.x recommended)
- OpenCV (cv2)
- NumPy
- argparse

You can install these dependencies using the following command:

```bash
pip install opencv-python numpy argparse
```

## Usage

1. Clone or download this repository to your local machine.
2. Open a terminal or command prompt and navigate to the directory containing the downloaded code.
3. Run the script with the following command:

For image:
```bash
python script.py --image path/to/your/image.jpg
```

For video (use webcam):
```bash
python script.py
```

Replace `path/to/your/image.jpg` with the actual path to the image you want to analyze.

## How it Works

1. The code reads the input image or video frame.
2. It uses a pre-trained deep learning model to detect faces in the image/video frame.
3. For each detected face, the code extracts the face region and preprocesses it.
4. The preprocessed face is then passed through two separate models: one for gender prediction and another for age estimation.
5. The code displays the original image/video frame with bounding boxes around detected faces and annotations indicating the predicted age and gender.

## Notes

- The `faceProto` and `faceModel` variables should point to the paths of the pre-trained face detection model files.
- The `ageProto` and `ageModel` variables should point to the paths of the pre-trained age estimation model files.
- The `genderProto` and `genderModel` variables should point to the paths of the pre-trained gender prediction model files.

## Acknowledgments

This code uses the OpenCV library and pre-trained models for face detection, age estimation, and gender prediction.

