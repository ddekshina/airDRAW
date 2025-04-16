# airDRAW
The "airDRAW" project is  a cross-platform web application that provides an intuitive, real-time, feature-rich, and accessible drawing experience using real-time hand gesture recognition and webcam input for interactive drawing and editing functionalities like drawing tools, text recognition, and shape detection across various devices.

## Features:

- Hand gesture-based drawing input.
- Real-time drawing and interaction.
- Various drawing tools and options.
- Shape and text recognition.
- Undo/redo, save/load, and download.
- Web-based and cross-platform.
- Backend hand tracking and gesture recognition (OpenCV, MediaPipe).
- Real-time WebSocket communication (Flask-SocketIO).

## Workflow:
1. User accesses web app.
2. Backend starts camera and tracking.
3. Frontend loads UI and connects via WebSocket.
4. Backend sends hand data and video.
5. Frontend interprets data for drawing and features.
6. User interacts with UI and drawing canvas.
7. Saving, loading, and downloading available.
   
## 4. Tech Stack Used
*   **Languages:**
    *   Python
    *   JavaScript
    *   HTML
    *   CSS

*   **Frameworks/Libraries/Tools:**

    *   **Backend:**
        *   Flask: Web framework for the server-side logic.
        *   Flask-SocketIO: For real-time, bidirectional communication using WebSockets.
        *   cv2 (OpenCV): For webcam video capture, frame processing and encoding.
        *   mediapipe: For hand tracking and landmark detection.
        *   eventlet: An asynchronous networking library that provides multithreading and WebSocket functionality.
        *   threading: For a separate thread for hand tracking.
        *   JSON: For serializing and deserializing data over WebSockets.
        *   base64: For encoding video frames for transmission.
        *   `requirements.txt` : Python package dependency management.

    *   **Frontend:**
        *   HTML5 Canvas API: Core drawing and manipulation technology.
        *   Socket.IO: For real-time communication with the backend.
        *   Tesseract.js: Optical Character Recognition (OCR) in the browser.
        *   CSS and CSS Variables: For styling and theming.
        *   No direct usage of frontend frameworks (React, Vue, Angular) is observed from the provided code.
        *   simplify-js : For simplifying the drawn shapes and lines.

