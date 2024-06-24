# AI-Speech-to-text-form-filling-
This application transcribes audio input, uses AI to fill forms based on the transcription, and prompts users for additional information if needed.
### App Description

Our app processes voice input using OpenAI Whisper API, transcribes it into text, and uses Gemini AI to extract and fill form data. Users can add more information via text or additional voice inputs, ensuring complete and accurate form submission.

### README

## Speech-to-Text and Form Filling Application

This application transcribes audio input, uses AI to fill forms based on the transcription, and prompts users for additional information if needed.

### Features

- Record or upload audio for transcription.
- Transcribe audio using OpenAI Whisper API.
- Use Gemini AI to fill form fields based on transcription.
- Fetch forms from Firebase Firestore.
- Prompt users for additional information if required.

### Prerequisites

- Node.js
- Python 3.x
- Firebase account
- OpenAI Whisper API and Gemini API keys

### Installation

1. **Clone the repository:**
   ```sh
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Set up the frontend:**
   ```sh
   cd frontend
   npm install
   ```

3. **Set up the backend:**
   ```sh
   cd ../backend
   pip install -r requirements.txt
   ```

4. **Configure environment variables:**

   Create a `.env` file in the backend directory with the following content:
   ```env
   REACT_APP_FIREBASE_API_KEY=<your_firebase_api_key>
   REACT_APP_GEMINI_API_KEY=<your_gemini_api_key>
   ```

### Running the Application

1. **Start the backend server:**
   ```sh
   cd backend
   uvicorn server:app --reload
   ```

2. **Start the frontend application:**
   ```sh
   cd frontend
   npm start
   ```

### Usage

1. **Record or upload audio:**
   - Click on the "Start Recording" button to record audio or upload an audio file.

2. **Process audio:**
   - Click the "Process" button to transcribe the audio.

3. **Send transcription to Gemini:**
   - Enter a prompt and click "Send to Gemini" to process the transcription.

4. **Fetch and fill forms:**
   - Click "Fetch Forms" to retrieve forms from Firebase.
   - Select a form and click "Fill Form" to auto-fill using the transcription.
   - If additional information is needed, provide input as requested.

### License

This project is licensed under the MIT License.

For more details, refer to the project documentation.
