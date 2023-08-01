# Barcode Decoder README.md

This README.md file provides an overview and explanation of the Barcode Decoder code created by Harsh Gupta (Desparete Enuf). The code is written in Python using the OpenCV and pyzbar libraries to detect and decode barcodes from a live video feed or an image.

## Getting Started

### Prerequisites

To run the Barcode Decoder code, you need to have Python installed on your system. Additionally, you'll need to install the following Python packages:

- OpenCV (`cv2`): A popular computer vision library for image and video processing.
- Numpy (`numpy`): A library for numerical computing in Python.
- pyzbar (`pyzbar`): A library for decoding barcodes from images.

You can install the required packages using the following command:

```bash
pip install opencv-python numpy pyzbar
```

### Running the Barcode Decoder

1. Clone or download the repository containing the Barcode Decoder code.
2. Ensure you have the required prerequisites installed.
3. Run the Python script, and the program will start capturing the video from your default camera (index 0).
4. Hold a barcode in front of the camera, and the program will attempt to detect and decode the barcode in real-time.
5. The detected barcode data and type will be printed to the console, and the barcode will be highlighted with a green polygon and label on the video feed.
6. Press 'q' to exit the program.

## Code Description

The Barcode Decoder code uses the OpenCV and pyzbar libraries to perform the following tasks:

1. Capture Video: The code uses OpenCV's `cv2.VideoCapture` to access the default camera and capture video frames.

2. Decode Barcodes: The `decoder` function takes an image as input and uses the pyzbar library to detect and decode any barcodes present in the image.

3. Draw Polygons and Labels: If a barcode is detected, the code draws a green polygon around the barcode region and displays the barcode data and type as a label on the video feed using OpenCV's drawing functions.

4. Real-time Processing: The code continuously processes each frame from the camera feed in real-time, attempting to detect and decode barcodes from the live video stream.

5. Exit: The program can be terminated by pressing the 'q' key.

## Dependencies

- `cv2`: The OpenCV library is used for image and video processing.
- `numpy`: Numpy is used for numerical computing and array operations.
- `pyzbar`: The pyzbar library is used for barcode detection and decoding.

## Acknowledgments

The Barcode Decoder code was created by Harsh Gupta (Desparete Enuf). The code utilizes the OpenCV and pyzbar libraries for barcode detection and decoding. The script demonstrates the use of real-time video processing with OpenCV in Python. This code can be useful for various applications, such as inventory management, QR code scanning, and more.

## License

This project is open-source and licensed under the [MIT License](LICENSE). You are free to modify and distribute the code, but please provide proper attribution to the original creator, Harsh Gupta (Desparete Enuf).
