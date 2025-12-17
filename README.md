# web_based_ai_assistant
🤖 My AI Assistant Hub
A lightweight, single-file AI dashboard powered by Google's Gemini 2.5 Flash model. This application serves as a personal hub for searching the web, planning tasks, and summarizing text—all within a clean, responsive interface styled with Tailwind CSS.

✨ Features
The application is divided into three distinct tools using a tabbed interface:

🌐 Smart Web Search:

Queries the Gemini API with Google Search grounding.

Returns up-to-date answers with citations and source links.

Displays a list of reference URLs for verification.

📅 Intelligent Planner:

Generates structured schedules, to-do lists, and project outlines.

Custom system instructions ensure output is organized and actionable.

📝 Text Summarizer:

Condenses long articles, emails, or documents into concise summaries.

Focuses on extracting key points and main ideas.

🛠️ Tech Stack
Frontend: HTML5, Native JavaScript (ES6+ Modules).

Styling: Tailwind CSS (loaded via CDN).

AI Model: Google Gemini 2.5 Flash (via Google AI Studio API).

Architecture: Serverless / Client-side only (No Node.js or Python backend required).

🚀 Getting Started
Since this is a single-file application, no build process (like Webpack or Vite) is required.

Prerequisites
You need a Google Gemini API key.

Go to Google AI Studio.

Create a new API Key.

Ensure the key has permissions for gemini-2.5-flash.

Installation
Clone the repository:

Bash

git clone https://github.com/yourusername/ai-assistant-hub.git
cd ai-assistant-hub
Configure your API Key:

Open ai_assistant.html in a code editor (VS Code, Notepad++, etc.).

Locate the configuration section near line 250:

JavaScript

// --- Configuration ---
const API_KEY = "YOUR_GEMINI_API_KEY_HERE";
Replace the placeholder with your actual API key.

Run the App:

Simply double-click ai_assistant.html to open it in your web browser.

Recommended: Use a lightweight local server (like Live Server in VS Code) to avoid CORS issues, though the file is designed to work standalone.

⚠️ Security Warning
Never commit your actual API key to GitHub.

If you plan to make this repository public:

Delete your API key from the code before pushing.

Replace it with a placeholder string (e.g., "PASTE_YOUR_KEY_HERE").

Consider using environment variables if you move this project to a build environment in the future.

🎨 Customization
You can easily tweak the look and feel by modifying the Tailwind classes in ai_assistant.html.

Theme: Change the background: linear-gradient(...) in the <style> tag to adjust the background colors.

Fonts: The app uses the "Inter" font family via Tailwind config.

Prompts: Modify the systemInstruction objects in the JavaScript logic to change how the Planner or Summarizer behaves (e.g., make the planner more strict, or the summarizer more casual).

📄 License
Distributed under the MIT License. See LICENSE for more information.

Note: This project uses the gemini-2.5-flash-preview model. API availability and naming conventions are subject to change by Google.
