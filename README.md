
Built by https://www.blackbox.ai

---

# Android Video Recorder App

## Project Overview
The Android Video Recorder App is a web-based application designed to simulate the functionality of a video recording application typically found on Android devices. It utilizes modern web technologies such as HTML, CSS, and JavaScript, providing features like user authentication and video recording capabilities—integrated with a simulated camera for testing purposes.

## Installation
To run the Android Video Recorder App locally, follow the steps below:

1. **Clone the repository**:
    ```bash
    git clone <repository_url>
    cd <repository_directory>
    ```

2. **Start the HTTP server**:
   Use Python's built-in HTTP server to serve the application:
   ```bash
   python3 -m http.server 8000
   ```
   This will serve the application at `http://localhost:8000`.

3. **Access the app**:
   Open your web browser and navigate to `http://localhost:8000` to start using the app.

## Usage
1. **Login**:
   - Enter your username and password on the login screen and click `Sign In`.

2. **Main Features**:
   - Navigate to the **Record Video** option to simulate video recording.
   - Access the **Gallery** feature to view saved recordings (currently prompts a future feature notice).
  
3. **Recording Video**:
   - Use the big red button to start and stop the recording.
   - Recorded videos will be displayed in a list below the recording display.

4. **Simulation Mode**:
   - If camera access is not available, the app will switch to simulation mode, indicating the camera is simulated for testing.

## Features
- User authentication with a login interface.
- Video recording functionality (simulated or real based on browser compatibility).
- Dynamic list that shows recent recordings.
- Simple and user-friendly interface designed with Tailwind CSS.

## Dependencies
This project uses several external libraries, which are loaded via CDN:
- [Tailwind CSS](https://tailwindcss.com/)
- [Font Awesome](https://fontawesome.com/)

No explicit dependencies are managed through a `package.json` file as this project is primarily an HTML/CSS/JS application.

## Project Structure
```
.
├── index.html              # Main HTML file for the application
```

### HTML File Breakdown
- **Head Section**: Contains metadata, stylesheets, and external libraries.
- **Body Section**:
  - **Android Status Bar**: Displays system information.
  - **Login Screen**: User inputs for authentication.
  - **Main Screen**: Navigation buttons for recording and accessing the gallery.
  - **Recording Screen**: Video playback area and controls for recording.

### JavaScript Functionality:
- Handles user login and navigation between the screens.
- Manages the video recording using the MediaRecorder API.
- Contains simulated behavior when camera access is denied.

---

For additional information or contributions, please refer to the project's GitHub repository.