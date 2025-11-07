# PikaBot Advanced

Piyangshu's Professional AI Chatbot powered by Google Gemini

## Description

A modern, feature-rich AI chatbot web application built with Node.js and Express, featuring text chat, image analysis, and file reading capabilities powered by Google's Gemini AI.

## Features

- **Text Chat**: Engage in natural conversations with AI
- **Image Analysis**: Upload and analyze images with detailed descriptions
- **File Reading**: Upload and analyze text files (TXT, PDF, DOC, DOCX)
- **Voice Input**: Support for voice messages (frontend ready)
- **Modern UI**: Clean, responsive chat interface with dark/light theme
- **Real-time Responses**: Fast AI-powered responses

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/pikabot-advanced.git
cd pikabot-advanced
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory and add your Google Gemini API key:
```
GEMINI_API_KEY=your_api_key_here
```

4. Start the development server:
```bash
npm run dev
```

Or start the production server:
```bash
npm start
```

The application will be running at `http://localhost:5000`

## Usage

1. Open your browser and navigate to `http://localhost:5000`
2. Start chatting with the AI assistant
3. Use the feature buttons to upload images or files for analysis
4. Toggle between light and dark themes using the moon icon

## API Endpoints

### POST /chat
Send a text message to the AI.

**Request Body:**
```json
{
  "message": "Hello, how are you?"
}
```

**Response:**
```json
{
  "reply": "I'm doing well, thank you for asking!"
}
```

### POST /analyze-image
Upload and analyze an image.

**Request:** Multipart form data with `image` file and optional `prompt`.

**Response:**
```json
{
  "reply": "Description of the image..."
}
```

### POST /read-file
Upload and analyze a text file.

**Request:** Multipart form data with `file` and optional `prompt`.

**Response:**
```json
{
  "reply": "Analysis of the document..."
}
```

### POST /generate-image
Placeholder for image generation (requires additional API integration).

## Technologies Used

- **Backend:** Node.js, Express.js
- **AI:** Google Generative AI (Gemini)
- **Frontend:** HTML5, CSS3, JavaScript (ES6+)
- **File Upload:** Multer
- **Styling:** Custom CSS with Font Awesome icons
- **Fonts:** Google Fonts (Inter)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**RN Sharma**

Made with ❤️ by Rudra
