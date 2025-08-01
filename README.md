# Japanese Interval Walking

<div align="left">
  <a href="https://htmlpreview.github.io/?https://raw.githubusercontent.com/tin2tin/Japanese_Interval_Walking/master/index.html">OPEN THE APP HERE</a><br><br>
</div>

A modern, touch-friendly web application designed to guide users through the scientifically-backed Japanese Interval Walking method. This app provides a clean, focused interface, pleasant audio cues, and detailed statistics to help users improve their fitness.

Built with pure HTML, CSS, and JavaScript, it is a lightweight, dependency-free Progressive Web App (PWA) that can be "installed" on any modern device.

## ✨ Features

- **Guided Interval Workouts**: The app guides users through a 30-minute workout consisting of 5 cycles of 3 minutes of fast-paced walking followed by 3 minutes of recovery pace.
- **Clean & Focused UI**: A minimalist design inspired by modern fitness apps, featuring a large timer and a dynamic progress ring.
- **Multilingual Support**: Fully translated into English, Danish, Spanish, Portuguese, and Chinese.
- **Voice & Audio Cues**:
    - Optional **Voice Coaching** provides verbal instructions for changing pace, milestones, and encouragement.
    - Non-verbal **tonal cues** signal pace changes and workout completion, usable with or without the voice coach.
    - "Silent mode" audio cues (a soft tick) for time remaining when the voice coach is disabled.
- **Automatic Step Counting**: Utilizes the device's accelerometer for real step counting. A fallback simulator is included for devices without sensor access.
- **Detailed Statistics**:
    - **Summary Card**: View your all-time total steps, fast steps, normal steps, and best day streak.
    - **7-Day Graph**: A bar chart visualizing your step count over the last week.
    - **Interactive Calendar**: See all your completed workout days at a glance and tap a day to view detailed session stats.
    - **Session Details**: Dive into a specific workout to see total steps and average cadence for fast and normal intervals.
- **Progressive Web App (PWA)**: Can be added to your home screen on both Android and iOS for a native app-like experience.
- **Responsive Design**: Looks and works great on desktops, tablets, and mobile phones. Includes a portrait-mode lock for a consistent experience on mobile.
- **Customization & Tools**:
    - **Debug Mode**: A 60-second workout mode for quick testing.
    - **Exit Button**: Easily close the app on supported PWA installations.

## 📸 Screenshots

| Main Screen | Main Screen | Statistics, Calendar & Session Details | About | Settings |
| :---: | :---: | :---: | :---: | :---: |
| <img width="518" height="883" alt="image" src="https://github.com/user-attachments/assets/74b4a73a-46d2-4290-86c7-227f9ddf4972" /> | <img width="513" height="889" alt="image" src="https://github.com/user-attachments/assets/0d067d25-4506-4051-a787-eee5bb4e14b3" /> | <<img width="517" height="886" alt="image" src="https://github.com/user-attachments/assets/5a92db25-bb22-4eef-898f-5f992fb6f8c7" /> | <img width="518" height="887" alt="image" src="https://github.com/user-attachments/assets/d39f244a-981a-4b71-9c88-16e48dce0aea" /> | <img width="517" height="887" alt="image" src="https://github.com/user-attachments/assets/72b0773c-f81f-4f8d-8504-effb3520f1ac" /> |


## 🚀 Getting Started

This is a pure client-side application and requires no build process.

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge).
- A web server for local development (to avoid CORS issues with `manifest.json`).

### Installation & Usage

1.  **Clone the repository:**
    ```sh
    git clone <your-repository-url>
    cd <repository-folder>
    ```

2.  **Run with a local server:**
    The easiest way to run the app locally is with a simple server.
    
    *   **Using VS Code:** Install the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension. Right-click on `index.html` and select "Open with Live Server".
    
    *   **Using Python:**
        ```sh
        # For Python 3
        python -m http.server
        ```

    *   **Using Node.js:**
        ```sh
        # Install serve globally if you don't have it
        npm install -g serve
        # Run from the project root
        serve
        ```

3.  Open your browser and navigate to the local address provided by your server (e.g., `http://localhost:8080`).

## ⚙️ How It Works

### The Workout Structure

The app is based on the Japanese Interval Walking method, which involves:
- **5 Cycles**: The entire 30-minute workout is composed of five identical cycles.
- **Each Cycle (6 minutes)**:
    - **3 minutes of High-Intensity Walking**: Aim for 70-80% of your maximum effort.
    - **3 minutes of Recovery Walking**: Slow down to a comfortable 40-50% effort.

This method is scientifically proven to be more effective at improving aerobic fitness and metabolic health than continuous walking at a moderate pace.

### Technology Stack

- **HTML5**: For the structure and content of the app.
- **CSS3**: For all styling, including Flexbox for layout, custom properties for theming, and media queries for responsiveness.
- **JavaScript (ES6+)**: For all application logic, including:
    - Timer management (`setInterval`).
    - **Web Audio API**: For generating pleasant, non-verbal sound cues.
    - **Speech Synthesis API**: For the voice coach functionality.
    - **Device Motion API / Accelerometer**: For step counting.
    - **`localStorage`**: For persisting user settings and workout history.
    - **PWA APIs**: `manifest.json` and Screen Orientation API for an installable, native-like experience.






