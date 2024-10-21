# Voice Bot: Capture and Playback Speech

This project demonstrates a simple speech recognition and text-to-speech (TTS) process using a Jupyter Notebook. The notebook captures speech from the microphone, converts it to text using Google's Speech Recognition API, and then speaks the recognized text back to the user using a text-to-speech engine.

## Features

- Captures audio input from the microphone.
- Converts speech to text using Google Speech Recognition API.
- Speaks the recognized text back to the user using `pyttsx3`.
- Error handling for unrecognized speech or API issues.

## Requirements

- Jupyter Notebook
- Python 3.x
- `speech_recognition` library
- `pyttsx3` library

## Usage

1. Run the cells in the notebook to initialize the necessary libraries and configurations.
2. The notebook will prompt you to speak into the microphone. Say something, and it will recognize your speech and repeat it back to you using the text-to-speech engine.

## Code Overview

The notebook contains a single function `recognize_and_speak(prompt)` which handles the entire process of speech recognition and TTS. Here's an overview of the workflow:

1. **Initialize Recognizer and TTS Engine**:
    - The `speech_recognition` library is used to capture and recognize speech.
    - The `pyttsx3` library is used to convert text to speech.

2. **Configure TTS Engine**:
    - The speaking rate is adjusted for clarity (50 words per minute slower).

3. **Capture Audio from Microphone**:
    - The microphone listens for input using the `speech_recognition` library's `Recognizer` class.

4. **Speech-to-Text Conversion**:
    - The captured audio is sent to Google's Speech Recognition API for transcription.

5. **Text-to-Speech Output**:
    - The recognized text is spoken back to the user using `pyttsx3`.

6. **Error Handling**:
    - Handles cases where speech is unrecognized or API issues occur, providing feedback to the user.
