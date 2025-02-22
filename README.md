# Voice Assistant with AI-Generated Responses

## Overview
This project is a voice assistant that listens to user input, processes it using Google's Gemini AI model, and responds with generated content via text-to-speech. It utilizes Python libraries for speech recognition, text-to-speech synthesis, and AI-generated responses.

## Features
- Listens to voice input using `speech_recognition`.
- Uses Google Speech Recognition to transcribe speech to text.
- Generates AI-based responses using Google Gemini AI (`gemini-pro`).
- Converts AI-generated text to speech using `pyttsx3`.
- Supports continuous conversation loop until the user says "exit".

## Prerequisites
Ensure you have Python installed (preferably Python 3.8+). You also need to install the required dependencies.

## Installation
1. Clone this repository or download the script.
2. Install dependencies:
   ```bash
   pip install speechrecognition pyttsx3 google-generativeai python-dotenv
   ```
3. Set up the environment variable for the API key:
   - Create a `.env` file in the project directory.
   - Add the following line, replacing `YOUR_GEMINI_API_KEY` with your actual API key:
     ```env
     GEMINI_API_KEY=YOUR_GEMINI_API_KEY
     ```

## Usage
Run the script using:
```bash
python script.py
```
The assistant will start listening. Speak into your microphone, and it will generate and read out responses. Say "exit" to terminate the program.

## Modules Used
- `os` - For environment variable handling.
- `dotenv` - To load environment variables from `.env` file.
- `speech_recognition` - For capturing voice input.
- `pyttsx3` - For text-to-speech conversion.
- `google-generativeai` - To interact with Google's Gemini AI.

## Notes
- Ensure your microphone is working properly.
- The model requires a valid API key for Google Gemini AI.
- Network connection is required for AI response generation.
