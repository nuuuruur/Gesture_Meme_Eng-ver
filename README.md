# Gesture Meme

A computer vision project that detects facial and hand gestures in real time using the webcam and displays a corresponding meme.

## Technologies

- **Python 3.10.0**
- **OpenCV**
- **MediaPipe**
- **NumPy**

## Requirements

- **Python 3.8 – 3.11** (MediaPipe is not compatible with later versions)

Install the dependencies using:

    pip install opencv-python mediapipe numpy

Or, if you have the requirements file:

    pip install -r requirements.txt

## Detected gestures

| Gesture | Meme |
|-------|------|
| **Raised or furrowed eyebrows** | `dog.jpeg` |
| **Tongue sticking out** | `cat1.png` |
| **Finger touching the mouth** | `cristiano.png` |
| **Both hands on either side of the face** | `face.jpeg` |
| **Both hands above the nose** | `Sonic.jpeg` |
| **Index and middle fingers extended** | `rat.jpeg` |

## Project structure

    gesture_meme/
    ├── main.py
    ├── requirements.txt
    ├── face.jpeg
    ├── cristiano.png
    ├── cat1.png
    ├── dog.jpeg
    ├── rat.jpeg
    └── Sonic.jpeg

## Usage

1. Clone the repository
2. Install the dependencies
3. Place the images in the same folder as `main.py`
4. Run:

       python main.py

5. When the programme starts, look straight ahead with a neutral expression during **calibration**
6. Once calibrated, try out the gestures in front of the camera
7. Press **ESC** to exit

## Notes

- **The calibration** takes a few seconds at the start; it is necessary for the gestures to work correctly
- The images must be in the **same folder** as `main.py`
- Works best with **good lighting**
- Compatible with **Windows** (uses `CAP_DSHOW` for the camera)
