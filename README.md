# Whisper-Audio-Transcription

**Overview**
This project provides an audio transcription interface using OpenAI's Whisper model. It allows users to upload or record audio and transcribes it into text using a Gradio-powered web interface.

**Features**
Supports audio file uploads

Uses OpenAI's Whisper model for accurate speech-to-text transcription

Handles various audio formats and sample rates

Deploys with a simple Gradio web interface

**Installation**
Ensure you have Python installed, then install the required dependencies:

pip install -U transformers torch torchaudio gradio soundfile librosa
Usage
Run the main script to start the transcription interface:
python script.py

**Code Structure**
Model Loading
Loads the Whisper model and processor from Hugging Face
Determines the appropriate device (CPU/GPU) for processing

**Audio Processing**
Loads and resamples audio to 16kHz
Ensures mono-channel audio for compatibility

**Transcription**
Converts processed audio into text using Whisper

**Gradio Interface**
Provides an interactive web interface for uploading or recording audio
Displays the transcribed text output

**Environment Variables**
This script expects an Hugging Face API token stored in an environment variable:
export HF_TOKEN=your_huggingface_token
