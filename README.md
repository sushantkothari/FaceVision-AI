# YOLOv8 Face Detection and Video Processing

An advanced project that leverages the YOLOv8 model for face detection in videos. This project uses Python-based libraries like OpenCV and NumPy to process video frames, detect faces, and annotate them with confidence scores and bounding boxes. It also provides options to save and display the processed video.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Workflow](#workflow)
- [Results](#results)
- [Dependencies](#dependencies)
- [Acknowledgments](#acknowledgments)

---

## Features

- **YOLOv8 Model**: Uses a specialized face detection model for high accuracy.
- **Video Processing**: Detects faces frame by frame in videos.
- **Bounding Boxes**: Annotates detected faces with bounding boxes and confidence scores.
- **Frame Details**: Displays frame numbers during processing.
- **Dynamic Visualization**: Allows displaying the processed video inline (for Jupyter/Colab environments).
- **Download Option**: Enables saving and downloading the processed video.

---

## Installation

To get started, ensure you have Python installed (version 3.8 or higher) and follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/yolov8-face-detection.git
   cd yolov8-face-detection
   ```

2. Install the required libraries:
   ```bash
   pip install ultralytics opencv-python numpy matplotlib scikit-image
   ```

3. Download the YOLOv8 face detection model:
   ```bash
   wget https://github.com/akanametov/yolov8-face/releases/download/v0.0.0/yolov8l-face.pt
   ```

---

## Usage

1. **Download an input video:**
   Update the video URL in the `gdown` command:
   ```bash
   !gdown --fuzzy https://drive.google.com/file/d/1nyeeqBJyDr2zphBDQ9ruh99JBdYm4nPH/view?usp=sharing --output test_video.mp4
   ```

2. **Run the script:**
   Execute the Python script to process the video:
   ```python
   python yolov8_face_detection.py
   ```

3. **Processed video output:**
   The processed video will be saved to the specified output path (default: `output_video_face.mp4`).

4. **Download and visualize:**
   If you're running this in a Jupyter/Colab environment, the processed video can be downloaded and displayed.

---

## Workflow

The face detection workflow consists of the following steps:

1. **Install Dependencies:** Install YOLOv8 and required Python libraries.
2. **Download the YOLOv8 Face Detection Model:** Use the specialized YOLOv8 face model for improved detection.
3. **Video Input:** Provide the path to the video file.
4. **Face Detection:** Process each frame using YOLOv8 and annotate detected faces.
5. **Save Output:** Save the annotated video to a file.
6. **Display Results:** Optionally visualize the processed video inline.

---

## Results

Below is an example of the output:

- **Input Video**: A raw video file containing faces.
- **Processed Video**: The output video with bounding boxes around detected faces, annotated with confidence scores.  

---

## Dependencies

This project relies on the following Python libraries:

- **[Ultralytics](https://github.com/ultralytics)**: For YOLOv8 face detection.
- **[OpenCV](https://opencv.org/)**: For video and image processing.
- **[NumPy](https://numpy.org/)**: For numerical operations.
- **[Matplotlib](https://matplotlib.org/)**: For visualizing video frames.
- **[Scikit-Image](https://scikit-image.org/)**: For resizing images.
- **[IPython](https://ipython.org/)**: For displaying the processed video inline.

---

## Acknowledgments

- **[YOLOv8 Face Model](https://github.com/akanametov/yolov8-face):** Special thanks to the contributors of the YOLOv8 face detection model for providing a robust tool for face detection.
- **Google Colab:** Used for easy execution and visualization.
- **OpenCV Team:** For their incredible library that simplifies video processing tasks.

---

## Contributing

Contributions are welcome! Feel free to fork this repository, make improvements, and submit a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

