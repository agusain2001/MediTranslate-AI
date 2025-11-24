# MediTranslate AI

MediTranslate AI is a real-time multilingual translation web app built for healthcare settings. It uses Google Gemini's multimodal AI to process raw audio with high accuracy, even when accents or medical terms are involved.

## Features

* **Multimodal voice recognition:** Uses Gemini 2.5 Flash to process audio directly for accurate medical transcription and translation.
* **Real-time contextual translation:** Captures meaning, tone, and intent for both doctors and patients.
* **Dual-role interface:** Separate controls for doctor (Speaker) and patient (Listener) languages.
* **Hybrid input modes:**

  * Voice recording
  * Manual text input with auto-debounced translation
  * Text-to-speech playback
* **Privacy-focused design:** No data is stored. Everything is processed in memory.

## Tech Stack

* **Frontend:** React (Vite)
* **AI Engine:** Google Gemini API (gemini-2.5-flash-preview-09-2025)
* **Styling:** Tailwind CSS with Lucide React icons
* **Audio:** MediaRecorder API + Blob handling
* **Deployment:** Works with Vercel or Netlify

## Prerequisites

* Node.js 18+
* npm
* Google Gemini API key

## Installation

### 1. Clone the repository

```
git clone https://github.com/your-username/meditranslate-ai.git
cd meditranslate-ai
```

### 2. Install dependencies

```
npm install
```

### 3. Configure environment variables

Create a `.env` file:

```
touch .env
```

Add your API key:

```
VITE_GOOGLE_API_KEY=AIzaSy...Your_Actual_API_Key_Here...
```

### 4. Start the development server

```
npm run dev
```

Open your browser at:

```
http://localhost:5173
```

## Usage

### Voice translation

1. Choose the speaker and listener languages.
2. Press the microphone button.
3. Speak and press stop when done.
4. The app will transcribe and translate.

### Text translation

Type in the original transcript box. Translation starts after one second of inactivity.

### Audio playback

Click the speaker icon to play the translated text as audio.

## Privacy

* No database or persistent storage.
* All API calls use HTTPS.
* Always confirm critical medical instructions with a qualified interpreter.

## Contributing

1. Fork the repo.
2. Create a branch.
3. Commit changes.
4. Push and open a pull request.

## License

This project is licensed under the MIT License.
