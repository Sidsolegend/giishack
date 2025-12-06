
LiveTranslate

A real-time speech-to-text + gesture recognition web app that combines the Web Speech API, webcam-based gesture detection, and a beautifully polished glassmorphic UI.

LiveTranslate allows users to speak into their microphone, see text updates live, train custom gestures, and run predictions directly in the browser — no backend required.

⸻

🚀 Features

🎙️ Live Speech Recognition
	•	Uses the Web Speech API for continuous speech-to-text.
	•	Real-time transcription displayed in a dedicated output panel.
	•	Interactive audio waveform generated via the Web Audio API.
	•	Start/stop listening with a single click.

✋ Gesture Recognition (ASL or Custom Gestures)
	•	Live webcam feed with adjustable canvas overlay.
	•	Users can:
	•	Enter a custom label
	•	Capture gesture samples
	•	Train a custom model directly in the browser
	•	Real-time prediction button to classify the current gesture.

📸 Camera System
	•	Live stream using getUserMedia().
	•	Status indicator (ACTIVE/ERROR).
	•	Hidden canvas used for gesture processing.

🖥️ Modern UI
	•	Fully glassmorphic interface.
	•	Smooth gradients, soft shadows, and responsive layout.
	•	Animated buttons with shimmer effect.
	•	Hover + focus transitions for professional feel.

⸻

🛠️ Tech Stack

-Area	Technology
-Speech Recognition	Web Speech API
-Audio Visualization	Web Audio API (AnalyserNode, Canvas)
-Gesture System	Webcam + Canvas capture
-Model Training	Browser-based JS (TensorFlow.js compatible)
-Frontend	Vanilla JavaScript, HTML5, CSS3
-Styling	Custom gradients, glassmorphism, responsive design


⸻

📦 Folder Structure (Recommended)

/LiveTranslate
│── index.html
│── style.css         # optional if separating styles
│── script.js         # optional if separating scripts
│── assets/
│     └── icons/
│     └── models/
└── README.md


⸻

▶️ How to Run
1.	Clone the repository:

        git clone https://github.com/yourusername/LiveTranslate.git

2.	Open the folder:

        cd LiveTranslate

3.	Simply open index.html in your browser.

No server needed — everything works client-side.

For gesture training to access your camera/mic, Chrome may require you to run from a local server.
Use this if necessary:

    python3 -m http.server

Then visit:
http://localhost:8000

⸻

✨ Core Functions Explained

🔊 startListening()
	•	Starts microphone recognition
	•	Begins drawing audio waveform
	•	Updates speech output live

🎥 Webcam + Gesture Capture
	•	Streams webcam into <video>
	•	Canvas grabs frames for model training
	•	Captured samples saved with a label

🤖 startTraining()
	•	Trains a small browser ML model
	•	Learns your custom gestures
	•	Updates UI after training

🔮 showPrediction()
	•	Runs inference on live video
	•	Displays predicted gesture label

⸻

🧪 Future Improvements
	•	TensorFlow.js integration for better accuracy
	•	Pretrained ASL model support
	•	Noise-robust speech recognition
	•	UI dark/light themes
	•	Save & load custom models

⸻

📄 License

MIT License — free to modify and distribute.

⸻

💬 Contributions

PRs are welcome!
You can improve:
	•	Model accuracy
	•	UI animations
	•	Documentation
	•	Cross-browser support

⸻

