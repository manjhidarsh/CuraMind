<div align="center">
	<img src="https://img.shields.io/badge/Python-3.12-blue?logo=python" alt="Python Version">
	<img src="https://img.shields.io/badge/License-MIT-green" alt="License">
</div>

# 🩺 CuraMind: AI Medical Assistant

CuraMind is a cutting-edge, multimodal AI-powered medical assistant designed to facilitate real-time medical diagnosis and patient interaction. By integrating advanced speech, text, and vision models, CuraMind delivers intelligent, interactive, and accessible healthcare support.

---

## Features

- **Multimodal AI**: Seamlessly combines speech recognition, image analysis, and natural language processing for comprehensive medical assistance.
- **Speech-to-Text (STT)**: Utilizes OpenAI Whisper for accurate voice transcription.
- **Vision Analysis**: Employs Llama 3 Vision for medical image interpretation.
- **AI Medical Reasoning**: Powered by Groq LLM for fast, context-aware responses.
- **Text-to-Speech (TTS)**: Converts AI responses to lifelike speech using ElevenLabs and gTTS.
- **Interactive UI**: Built with Gradio for an intuitive, real-time consultation experience.
- **Optimized Performance**: Enhanced with Groq API for up to 40% faster inference.

---

## Demo

https://github.com/manjhidarsh/CuraMind/assets/demo.gif <!-- Replace with actual demo link or remove if not available -->

---

## Getting Started

### Prerequisites
- Python 3.12+
- [Pipenv](https://pipenv.pypa.io/en/latest/) (recommended) or pip
- [ffmpeg](https://ffmpeg.org/) (for audio processing)
- [PortAudio](http://www.portaudio.com/) (for microphone input)
- GPU (optional, for faster inference)

### Installation

1. **Clone the Repository**
	 ```bash
	 git clone https://github.com/manjhidarsh/CuraMind.git
	 cd CuraMind
	 ```
2. **Install Dependencies**
	 ```bash
	 pipenv install
	 # or, if using pip:
	 pip install -r requirements.txt
	 ```
3. **Set API Keys**
	 - Set your `GROQ_API_KEY` and `ELEVENLABS_API_KEY` as environment variables:
		 - On Windows (PowerShell):
			 ```powershell
			 $env:GROQ_API_KEY="your_groq_api_key"
			 $env:ELEVENLABS_API_KEY="your_elevenlabs_api_key"
			 ```
		 - On Linux/macOS:
			 ```bash
			 export GROQ_API_KEY="your_groq_api_key"
			 export ELEVENLABS_API_KEY="your_elevenlabs_api_key"
			 ```

---

## Usage

Launch the Gradio app for an interactive AI-powered medical consultation:

```bash
python gradio_app.py
```

### Main Functionalities
- **Speak your symptoms**: AI transcribes and analyzes your voice input.
- **Upload a medical image**: Llama 3 Vision provides instant insights.
- **Receive AI-powered diagnosis**: Get concise, context-aware medical advice.
- **Hear responses**: Listen to lifelike speech output via ElevenLabs or gTTS.

---

## Project Structure

```
CuraMind/
├── brain_of_the_doc.py         # Image analysis and LLM integration
├── gradio_app.py              # Gradio UI for user interaction
├── voice_of_the_doc.py        # Text-to-speech (TTS) utilities
├── voice_of_the_patient.py    # Audio recording and speech-to-text (STT)
├── Pipfile                    # Dependency management
├── README.md                  # Project documentation
└── ...                        # Other assets and files
```

---

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements, bug fixes, or new features.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgements
- [Groq](https://groq.com/) for LLM and Whisper API
- [Llama 3 Vision](https://llama.meta.com/) for image analysis
- [ElevenLabs](https://elevenlabs.io/) and [gTTS](https://pypi.org/project/gTTS/) for TTS
- [Gradio](https://gradio.app/) for the UI framework
