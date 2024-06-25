# Hand AR Project

This project implements an Augmented Reality (AR) application that detects objects in an image or live video feed, allows the user to select an object, and then places that object on the user's hand in real-time.

## Features

- Object detection and segmentation using YOLO (You Only Look Once) model
- Interactive object selection from an image or live video feed
- Hand tracking using MediaPipe
- Real-time AR placement of selected objects on the user's hand

## Requirements

- Python 3.x
- OpenCV (cv2)
- NumPy
- MediaPipe
- Ultralytics YOLO

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/hand-ar-project.git
   cd hand-ar-project
   ```

2. Install the required packages:
   ```
   pip install opencv-python numpy mediapipe ultralytics
   ```

3. Download the YOLO model:
   ```
   wget https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m-seg.pt
   ```

## Usage

The project contains two main scripts:

1. Live Camera Mode:
   - Run the script in a Jupyter notebook or as a Python file.
   - The script will open your webcam and start object detection.
   - Click on an object to select it.
   - Press Enter to confirm your selection.
   - The selected object will appear on your hand in the AR view.
   - Press 'q' or 'Esc' to exit.

2. Directory Mode:
   - Place the image you want to use in the same directory as the script and name it "test.jpeg".
   - Run the script in a Jupyter notebook or as a Python file.
   - Click on an object in the image to select it.
   - Press Enter to confirm your selection.
   - The AR view will open, showing the selected object on your hand.
   - Press 'q' or 'Esc' to exit.

## How It Works

1. The script uses YOLO to detect and segment objects in the input image or video feed.
2. Users can interactively select an object by clicking on it.
3. The selected object is extracted and processed.
4. MediaPipe is used to detect and track the user's hand in real-time.
5. The extracted object is overlaid on the user's hand, creating an AR effect.

## Limitations

- The hand tracking may not work perfectly in all lighting conditions or with rapid hand movements.
- The AR placement is currently basic and does not account for hand orientation or lighting.

## Future Improvements

- Implement more advanced AR techniques for realistic object placement.
- Add support for multiple object selection and placement.
- Improve hand tracking stability and performance.
- Add gesture recognition for more interactive AR experiences.

## Contributing

Contributions to improve the project are welcome. Please feel free to fork the repository, make changes, and submit pull requests.


