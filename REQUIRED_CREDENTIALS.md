# Required n8n Credentials

To run the "AI Voice Agent" workflow successfully, you must create the following credentials in your n8n instance.

- **Service:** Twilio
  - **n8n Credential Type:** `Twilio`
  - **Required For:** Voice call handling (TwiML), sending SMS.
  - **Values Needed:** Account SID and Auth Token.

- **Service:** Deepgram
  - **n8n Credential Type:** `Deepgram`
  - **Required For:** Speech-to-text transcription.
  - **Values Needed:** API Key.

- **Service:** OpenAI
  - **n8n Credential Type:** `OpenAI`
  - **Required For:** AI-powered intent recognition and responses (GPT-4o).
  - **Values Needed:** API Key.

- **Service:** Stripe
  - **n8n Credential Type:** `Stripe`
  - **Required For:** Creating payment links.
  - **Values Needed:** API Key.

- **Service:** Google Cloud
  - **n8n Credential Type:** `Google`
  - **Required For:** Text-to-speech synthesis.
  - **Values Needed:** Service Account JSON file.

- **Service:** Supabase
  - **n8n Credential Type:** N/A (Handled via Environment Variable)
  - **Required For:** Storing generated audio files.
  - **Values Needed:** `SUPABASE_SERVICE_KEY` (to be set in the `.env` file).
