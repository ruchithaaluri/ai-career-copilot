# AI Career Copilot

An AI-powered, Gemini-powered resume analyzer and career assistant.

## Features

- Secure server-side Gemini API key (`.env` is not exposed to the browser)
- Custom app name and theme colors
- PDF resume upload and text extraction using PDF.js
- Resume analysis history saved in browser `localStorage`
- English/Hindi analysis-language toggle
- Export analysis reports to PDF
- Dark mode
- ATS alignment score estimate
- Missing keyword identification
- Actionable resume improvement suggestions
- Skill-gap analysis
- Salary estimate field

## Requirements

- Node.js 18 or newer
- Gemini API key from [Google AI Studio](https://aistudio.google.com/)

## Installation and Setup

1. Clone or download this repository.
2. Open the project folder in VS Code.
3. Open `.env` and replace `PASTE_YOUR_GEMINI_API_KEY_HERE` with your Gemini API key.
4. Open the VS Code terminal.
5. Install dependencies:

   ```bash
   npm install
   ```

6. Start the application:

   ```bash
   npm start
   ```

7. Open your browser and visit:

   `http://localhost:3000`

## Environment Variables

Configure your `.env` file:

```env
GEMINI_API_KEY=your_gemini_api_key
PORT=3000
GEMINI_MODEL=gemini-3.8-flash
```

Never share your actual API key.

## Security Notes

- Never commit `.env` or expose your Gemini API key.
- `.gitignore` excludes sensitive environment files.
- If a key is accidentally published, revoke it in Google AI Studio.
- Add authentication and rate limiting before public deployment.
- Resume text is sent to Gemini for analysis. Obtain permission before processing another person's resume.
- ATS scores and salary estimates are approximate.

## Troubleshooting

- **API key missing:** Check your `.env` file and restart the application.
- **Model error:** Check your Gemini model configuration and API access.
- **PDF upload or export not working:** Ensure internet access for PDF.js and jsPDF CDN libraries.
- **Port already in use:** Change `PORT=3000` to `PORT=3001` in `.env` and restart.

## Tech Stack

- HTML
- CSS
- JavaScript
- Node.js
- Express.js
- Google Gemini API
- PDF.js
- jsPDF

## Author

Developed as an AI-powered career assistance project.