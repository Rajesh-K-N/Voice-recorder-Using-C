# Voice-recorder-Using-C
Here's a **README.md** file for your **Voice Recorder** project. It includes details about the project, setup instructions, usage, and technical specifications.  

Let me know if you need modifications!  

---

### 📜 **README.md**  

```markdown
# 🎤 Voice Recorder

## 📌 Project Overview
The **Voice Recorder** is a web-based application that allows users to record and manage audio recordings. The application is built using **Flask** for the backend and **C** for audio recording, which ensures high-performance sound capture. The frontend is designed with **HTML, CSS, and JavaScript** to provide a user-friendly experience.

## 🛠️ Features
- 🎙️ **Record Audio:** Users can specify a duration and record their voice.
- 🎵 **Playback Recordings:** Listen to previous recordings through an embedded audio player.
- 📂 **Download Audio Files:** Easily download recorded audio in WAV format.
- ❌ **Error Handling:** Friendly UI for error messages.

---

## 🚀 Installation & Setup

### 1️⃣ Prerequisites
Ensure you have the following installed on your system:
- 🐍 **Python 3.8+**
- 📦 **Flask** (install using `pip install flask`)
- 💻 **Windows OS** (for the C-based recorder)
- 🎤 **Microphone** (required for recording)

### 2️⃣ Clone the Repository
```sh
git clone https://github.com/your-repo/voice-recorder.git
cd voice-recorder
```

### 3️⃣ Install Dependencies
```sh
pip install flask
```

### 4️⃣ Run the Application
```sh
python app.py
```
By default, the server will start on **`http://127.0.0.1:5000/`**.

---

## 📂 Project Structure
```
📁 voice-recorder
│── app.py               # Flask application (backend)
│── voice_recorder.c      # C program for recording audio
│── voice_recorder.exe    # Compiled executable for recording (Windows only)
│── templates/
│   ├── index.html        # Main page (record audio, view recordings)
│   ├── player.html       # Audio player for playback
│   ├── error.html        # Error display page
│── static/               # (Optional: for CSS/JS files)
│── Recordings/           # Directory where recordings are saved
│── README.md             # Documentation
```

---

## 🎮 How It Works

1️⃣ **Recording Audio**
   - Open the app (`http://127.0.0.1:5000/`).
   - Enter the duration in seconds.
   - Click **"Start Recording"** (this runs the C program `voice_recorder.exe`).

2️⃣ **Playing Audio**
   - Select a recorded file from the list.
   - Click **"Play"** to listen to the recording.

3️⃣ **Downloading Recordings**
   - Click **"Download"** to save the file.

---

## 🛠️ Technical Details

### 📌 Backend (Flask)
- Handles routing, recording, playback, and file management.
- Uses `subprocess` to call the C executable for recording.

### 📌 Frontend (HTML, CSS, JS)
- Dynamic UI with Bootstrap-like styles.
- Embedded audio player with a **playback visualizer**.

### 📌 C Program (`voice_recorder.c`)
- Uses **Windows Audio APIs** to capture sound.
- Saves audio in **WAV format**.
- Runs via `voice_recorder.exe`.

---

## 📌 Known Issues & Limitations
- ❗ **Windows-Only:** The recorder (`voice_recorder.exe`) works only on Windows.
- 🎤 **Microphone Required:** Ensure the mic is connected.
- ⏳ **Recording Time Limit:** Max 300 seconds per recording.

---

## 👨‍💻 Author
- **Rajesh K N**
- 📧 Contact: rajeshkuliyakanda@gmail.com

---
```
