

# AI Content Safety Simulator via Claude

The **AI Content Safety Simulator** is a lightweight web-based tool that analyzes text input and classifies it as **SAFE**, **NEUTRAL**, or **UNSAFE**. It highlights the presence of negative, neutral, or positive words and provides a structured JSON-style result.

---

## Features
- **Text Classification**: Detects unsafe, neutral, and safe text based on predefined word lists.  
- **Interactive UI**: Enter text and instantly see the analysis.  
- **Results Panel**: Displays structured JSON with classification status and word counts.  
- **Responsive Design**: Built with modern HTML, CSS, and JavaScript for browser-based use only.  
- **Customizable**: Word lists can be expanded or tailored for different content safety use cases.  

---

## Word Categories
- **Negative Words (60 total)**: Examples – `kill`, `murder`, `attack`, `hate`, `fraud`  
- **Neutral Words (60 total)**: Examples – `confused`, `plan`, `review`, `observe`, `analyze`  
- **Positive Words (60 total)**: Examples – `love`, `happy`, `peace`, `support`, `joyful`  

---

## How It Works
1. Type or paste text into the input box.  
2. Click **Check Content**.  
3. The script counts matches from the three word lists.  
4. A JSON-style result is displayed showing:
   - `status`: SAFE / NEUTRAL / UNSAFE  
   - `input`: the original text  
   - `analysis`: count of detected words per category  
   - `ai_safe`: Boolean indicating if the text is considered safe  

---
Try: https://pritiks23.github.io/Claude-Content-Safety/

## Example Output
```json
{
  "status": "UNSAFE",
  "input": "This is a dangerous attack",
  "analysis": {
    "negative_words_found": 2,
    "neutral_words_found": 0,
    "positive_words_found": 0
  },
  "ai_safe": false
}
