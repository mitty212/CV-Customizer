# 📄 CV Customizer — Chrome Extension

**CV Customizer** is a Chrome extension that uses AI (via OpenRouter) to generate a tailored professional summary for your resume based on any job posting page you're currently viewing. It automatically replaces a placeholder tag in your `.docx` resume and exports a customized file ready to submit.

---

## ⚡ Prerequisites

1. An **OpenRouter API Key** (get one at [openrouter.ai](https://openrouter.ai/)).
2. A `.docx` resume file containing the placeholder tag `[CV Customize]` where you want your professional summary to appear.

---

## 📥 Installation

1. **Download or clone** this repository to your computer.
2. Open Google Chrome and go to `chrome://extensions/`.
3. Enable **Developer mode** (toggle in the top-right corner).
4. Click **Load unpacked** in the top-left corner.
5. Select the project folder containing `manifest.json`.

---

## 🚀 How to Use

### Step 1: Prepare Your Resume Template
Open your resume in Microsoft Word or Google Docs and type **`[CV Customize]`** exactly where your professional summary should be located. Save it as a `.docx` file.

### Step 2: Configure the Extension
1. Click the **CV Customizer** icon in your Chrome extension toolbar.
2. Enter your **OpenRouter API Key**.
3. Choose an **AI Model** (or pick *Other (custom model)...* and enter a valid model ID like `google/gemini-2.5-flash`).
4. Type your **Base Professional Summary** (your standard summary to give the AI context about your background).
5. Upload your `.docx` resume template. *(Your settings and resume are saved locally in Chrome so you don't need to upload every time!)*

### Step 3: Generate Tailored CV
1. Navigate to any job posting page on the web (LinkedIn, Indeed, company careers page, etc.).
2. Click the **CV Customizer** icon.
3. Click **Create Custom CV**.
4. The extension will read the job posting, generate a tailored summary matching the job requirements, insert it into your `.docx` file, and provide a download link!

---

## 🛠️ Features

- 🎯 **Tailored Summaries**: Matches your resume details with the specific job posting requirements.
- 💾 **Local Persistence**: Saves your API key, settings, and base resume template securely in `chrome.storage.local`.
- 🤖 **Flexible AI Support**: Works with standard models (Gemini, Claude, GPT-4, DeepSeek) or any custom OpenRouter model ID.
- 📄 **Format Preservation**: Replaces `[CV Customize]` in your `.docx` document while retaining your formatting and styles.
