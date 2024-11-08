# driver_drowsiness_detection
# Driver Drowsiness Detection

This project detects driver drowsiness in real-time using facial landmark detection to monitor eye blinks and classify driver states as **Active**, **Drowsy**, or **Sleeping**.

## Code Explanation

### Libraries and Dependencies
- **OpenCV (cv2)**: Used for handling video capture and image processing.
- **NumPy**: Provides numerical functions to calculate distances between facial landmarks.
- **Dlib**: Detects faces and landmarks.
- **face_utils (from imutils)**: Simplifies facial landmark manipulation.

### Workflow
1. **Setup and Initialization**
   - Initializes camera, face detector, and landmark predictor with Dlib.

2. **Functions**
   - **`compute`**: Calculates the distance between two points.
   - **`blinked`**: Calculates Eye Aspect Ratio (EAR) to classify eyes as open, drowsy, or closed.

3. **Main Detection Loop**
   - Captures frames, detects faces, and processes landmarks to classify driver state as **Active**, **Drowsy**, or **Sleeping** based on eye state.

4. **Status Display**
   - Shows **Active** (green), **Drowsy** (blue), or **Sleeping** (red) on-screen status.

5. **Exit Mechanism**
   - The loop ends when “Esc” is pressed.

This code helps monitor driver alertness and can be part of an advanced driver assistance system (ADAS).
