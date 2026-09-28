# oaqjp-final-project-emb-ai
# Final Project: Emotion Detection Application

**Project Name:** Emotion Detection Application

An AI-powered web application that analyzes the emotional tone of text input using IBM Watson NLP and presents the emotional profile along with the dominant emotion through a responsive Flask web interface.

---

## 📌 Project Overview

This project implements an end-to-end AI application for emotion analysis:
- **Project Name**: Emotion Detection Application (`oaqjp-final-project-emb-ai`)
- **Core AI Engine**: Uses IBM Watson NLP EmotionPredict library to predict emotional scores for `anger`, `disgust`, `fear`, `joy`, and `sadness`, determining the `dominant_emotion`.
- **Modular Architecture**: Packaged into a reusable Python module `EmotionDetection`.
- **Unit Testing**: Verified with `unittest` across diverse emotional statements.
- **Web Interface**: Deployed with **Flask**, featuring asynchronous API calls and dynamic UI updates.
- **Error Handling**: Gracefully handles blank and invalid inputs returning status code 400 with user-friendly notices.
- **Static Code Analysis**: Fully styled and documented to achieve a perfect **10.00/10** score on `pylint`.

---

## 🗂️ Project Structure

```text
oaqjp-final-project-emb-ai/
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
├── static/
│   └── mywebscript.js
├── templates/
│   └── index.html
├── test_emotion_detection.py
├── server.py
├── README.md
└── requirements.txt
```

---

## 🚀 Setup & Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Harshjoshi211/oaqjp-final-project-emb-ai.git
   cd oaqjp-final-project-emb-ai
   ```

2. Install dependencies:
   ```bash
   pip install flask requests pylint
   ```

3. Run unit tests:
   ```bash
   python test_emotion_detection.py
   ```

4. Run static code analysis:
   ```bash
   pylint server.py
   ```

5. Start the web application:
   ```bash
   python server.py
   ```
   Open your browser and navigate to `http://localhost:5000/`.

---

## 📊 Sample Output

For input text: *"I love my life"*
```text
For the given statement, the system response is 'anger': 0.0076241386, 'disgust': 0.0016488214, 'fear': 0.0039234855, 'joy': 0.9632832 and 'sadness': 0.038475268. The dominant emotion is joy.
```

---

## 📄 License
This project is licensed under the Apache License 2.0.
