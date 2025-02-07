# Hand Tracking with MediaPipe

## Overview
This project utilizes **MediaPipe** and **OpenCV** to track hand landmarks in real-time using a webcam or static images. The script detects hands, draws keypoints, and displays the processed video feed with landmark annotations.

## Features
- Detect and track hand landmarks in real-time
- Process static images for hand landmark detection
- Identify handedness (left/right hand)
- Display index finger tip coordinates
- Overlay hand connections and landmarks on the image
- Flip the image for a selfie-view display

## Libraries Required
The following Python libraries are needed:

1. **OpenCV** (`cv2`) - For image and video processing
2. **MediaPipe** (`mediapipe`) - For hand tracking and landmark detection

## Installation
Ensure you have Python installed, then install the required dependencies:

```bash
pip install opencv-python mediapipe
```

## Usage
### Running the Script for Real-Time Webcam Tracking
```bash
python hand_tracking.py
```

### Running the Script for Static Image Processing
Modify `IMAGE_FILES` in the script to include the path to your images, then run:
```bash
python hand_tracking.py
```

## Code Explanation
- **Static Image Processing:** Reads and flips images, converts them to RGB, and processes them to detect hands.
- **Real-Time Tracking:** Captures video from the webcam, processes each frame, detects hand landmarks, and displays the output.
- **Drawing Utilities:** Uses `mp_drawing` to visualize detected hand connections and key landmarks.

## Example Output
When running the script, you will see a real-time webcam feed with detected hand landmarks drawn. Press `Esc` to exit the program.

## Contributing
Feel free to contribute by improving the code or optimizing hand detection!

## License
This project is licensed under the MIT License.

