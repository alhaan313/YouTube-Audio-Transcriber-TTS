YouTube Video Downloader, Transcriber, and Audio Generator
This project automates the process of downloading a YouTube video, extracting its audio, transcribing it using Deepgram's API, and generating synthesized speech with ElevenLabs.

Features
Download YouTube videos and extract audio.
Transcribe audio using Deepgram's speech-to-text API.
Convert the transcript into audio using ElevenLabs' Text-to-Speech.
Automatically save the processed files in specified directories.
Project Structure
pytubefix: Used for downloading YouTube videos and extracting audio.
Deepgram API: Transcribes the extracted audio.
ElevenLabs API: Converts the transcript into synthesized audio.
pydub: Handles audio file conversion (e.g., from different formats to MP3).
Setup
Requirements
Python 3.7 or above.
Install required Python libraries (refer to requirements.txt).
Installation
Clone this repository:

bash
Copy code
git clone https://github.com/yourusername/yourrepo.git
cd yourrepo
Install the required dependencies:

bash
Copy code
pip install -r requirements.txt
Create necessary directories for saving videos and audio:

bash
Copy code
mkdir -p /content/videos
mkdir -p /content/audio
Environment Variables
You'll need API keys for Deepgram and ElevenLabs to use their services. Store these API keys in Google Colab’s userdata or replace the relevant code parts with direct API key inputs.

Deepgram API Key: Store it as Deepgram_ApiKey.
ElevenLabs API Key: Store it as ElevenLabs_ApiKey.
Running the Program
Ensure you have the correct video link and paths configured:

python
Copy code
link = "https://www.youtube.com/watch?v=1aA1WGON49E"
SAVE_PATH = "/content/videos"
AUDIO_PATH = "/content/audio"
Run the script to download, transcribe, and generate audio.

Outputs
Downloaded Video: Saved in /content/videos.
Extracted Audio (MP3): Saved in /content/audio.
Generated Audio from Transcript: Saved in /content/generated_audio.
Dependencies
See requirements.txt for Python library dependencies.

License
This project is licensed under the MIT License.
