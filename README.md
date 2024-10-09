# SIGNLINK : Sign Language Detection and Translation Application

This Flask application utilizes computer vision techniques to detect hand signs and provide real-time translation. The application leverages MediaPipe for hand landmark detection and a custom keypoint classifier to recognize hand signs. It also features two modes: one for learning gestures and another for translating them into text.

## Features

- **Hand Sign Detection**: Uses a webcam to capture hand movements and recognize specific hand signs.
- **Gesture Learning**: Allows users to learn different gestures.
- **Sign Translation**: Translates recognized signs into text.
- **Real-time Video Streaming**: Displays the camera feed with detected hand signs and relevant information.

## Requirements

- Python 3.x
- Flask
- OpenCV
- MediaPipe
- Other dependencies specified in `requirements.txt`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/hammadali1805/SignLink.git
   cd SignLink
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Make sure to update any paths in the code if needed.

## Usage

1. Start the Flask application:
   ```bash
   python my_app.py
   ```

2. Open your web browser and navigate to `http://127.0.0.1:5000/`.

3. Use the following endpoints:
   - `/` - Home page
   - `/learn` - Learning mode for hand signs
   - `/translate` - Translation mode for hand signs
   - `/sign` - Get the currently selected sign
   - `/detectedsign` - Get the detected sign
   - `/video/<usecase>` - Real-time video streaming (use `learn` or `translate` as the use case)

## Controls

- Use keys `0-9` to select different hand signs.
- Press `n` to switch to learning mode.
- Press `k` to switch to translation mode.
- Press `h` for help or information about current modes.
- Press `ESC` to exit the application.

## Acknowledgments

- MediaPipe: https://google.github.io/mediapipe/
- OpenCV: https://opencv.org/
- Other resources and libraries utilized in the project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
