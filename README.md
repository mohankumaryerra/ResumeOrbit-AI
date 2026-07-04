# AI Resume Analyzer

An industry-grade, client-side web application that uses Google's Gemini API to analyze resumes, provide ATS scoring, identify keyword gaps, and rewrite bullet points for maximum impact.

![AI Resume Analyzer Preview](https://via.placeholder.com/1200x630.png?text=AI+Resume+Analyzer)

## Features

- **ATS Scoring & Section Breakdown:** Get quantitative scores for your overall resume, experience, education, skills, and formatting.
- **AI Bullet Rewriter:** Automatically identify weak bullet points and get AI-rewritten suggestions with action verbs and metrics.
- **Keyword Gap Analysis:** Identify missing keywords based on your target role and job description.
- **Career Advisor:** Get personalized interview questions and alternative job role suggestions based on your profile.
- **Persistent History:** Automatically saves your last 5 analyses in your browser.
- **Export Options:** Download your analysis report as a JSON or TXT file, or print it as a polished PDF.
- **Privacy First:** All parsing (PDF/DOCX/TXT) happens locally in your browser. The text is sent directly to Google's Gemini API using your personal API key. No intermediate servers are used.

## Tech Stack

- **Frontend:** Vanilla HTML, CSS (Glassmorphism design), and JavaScript.
- **AI Model:** Meta Llama 3.3 70B (via OpenRouter).
- **File Parsing:** 
  - `pdf.js` for PDF extraction.
  - `mammoth.js` for DOCX extraction.
- **Visualizations:** `Chart.js` for animated score rings.

## Running Locally

Because this is a purely client-side application, you can run it simply by opening `index.html` in your browser. However, for the best experience (and to avoid any potential CORS issues with local files), running a local server is recommended.

### Prerequisites

You will need an [OpenRouter API Key](https://openrouter.ai/keys).

### Quick Start

1. Clone or download the repository.
2. Open your terminal in the project directory.
3. Start a local server:
   - Using Python: `python -m http.server 8000`
   - Using Node.js: `npx serve .`
4. Open your browser and navigate to the local server URL (e.g., `http://localhost:8000` or `http://localhost:3000`).
5. Enter your OpenRouter API key in `js/config.js` and upload a resume!

## Demo Mode

Don't have a resume handy? Click the **"Try with Sample"** button on the landing page to instantly see what a comprehensive analysis looks like using mock data.
