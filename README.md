# YouTube Video Summarizer with Speech Synthesis

Welcome to the **YouTube Video Summarizer with Speech Synthesis** repository! This project provides a fully automated solution to fetch YouTube videos, transcribe their audio content, summarize the transcriptions, and convert the summary into audio. You can receive daily summaries of your favorite YouTube channels delivered directly to your inbox!

### Features:
- **Fetch Videos from YouTube**: Automatically fetch the latest videos from a specified YouTube channel.
- **Audio Download and Transcription**: Download audio from YouTube videos, split the audio into chunks, and transcribe using speech recognition.
- **Text Summarization**: Summarize transcribed text using state-of-the-art NLP models.
- **Text-to-Speech**: Convert the summarized text into natural-sounding audio using ElevenLabs’ AI-powered voice generation.
- **Email Notifications**: Receive an email with video summaries and audio attachments of the video summaries.

### Key Technologies:
- **YouTube Data API**: Fetch videos from a specified channel.
- **Speech Recognition**: Transcribe YouTube video audio using the Google Speech-to-Text API.
- **Transformers**: Summarize the transcribed text using NLP models from Hugging Face.
- **ElevenLabs**: Convert summarized text into speech.
- **Email**: Send email notifications with video summaries and audio attachments.

### How It Works:
1. The script fetches the latest videos from the specified YouTube channel using the YouTube Data API.
2. It downloads the audio of these videos and transcribes them using speech recognition.
3. The transcriptions are then summarized using an NLP model.
4. The summary is converted into speech using ElevenLabs' text-to-speech service.
5. Finally, the summary and its audio version are sent via email to the user.

### Setup Instructions:
1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/YouTube-Video-Summarizer.git
   cd YouTube-Video-Summarizer

2. Install the required dependencies:
   pip install -r requirements.txt

3. Set up your environment variables. Create a .env file in the root directory and add your API keys and credentials:

   ```bash
   API_KEY=your_youtube_data_api_key
   ELEVEN_API_KEY=your_elevenlabs_api_key
   EMAIL_PASSWORD=your_email_password

5. Run the script to start processing videos from the channel:

   ```bash
   python your_script_name.py

7. You will receive daily email summaries with audio attachments.



## Example Usage:
- To process videos from a specific channel and get daily summaries:

  ```bash
  CHANNEL_ID = 'your_channel_id'
  process_videos(CHANNEL_ID, days=7)


## Contributing:
We welcome contributions! If you have any improvements, bug fixes, or features in mind, feel free to fork the repository and submit a pull request.

## License:
This project is licensed under the MIT License - see the LICENSE file for details.


