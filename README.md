# 🤖 Gemini One-Line Chatbot with Mood Score

A terminal-based chatbot that interacts using Google’s Gemini API and evaluates the user's emotional tone using a HuggingFace NLP model. At the end of the chat session, it provides a **Final Mood Score** and highlights the **Dominant Mood** from a simplified set: `Happy`, `Calm`, `Confused`, `Sad`, `Angry`.

---

## 🚀 Features

- ✅ Gemini-powered single-line chatbot replies  
- ✅ Terminal-based chat loop  
- ✅ NLP-based emotion detection using `distilBERT`  
- ✅ Simplified mood categorization (5 categories)  
- ✅ Final score based on all user inputs  

---

## 🧠 Technologies Used

| Layer      | Tech |
|------------|------|
| Chatbot    | [Google Generative AI - Gemini](https://ai.google.dev/) |
| NLP Model  | [HuggingFace Transformers](https://huggingface.co/bhadresh-savani/distilbert-base-uncased-emotion) |
| Language   | Python 3.8+ |

---

## 🛠️ Setup Instructions

### ✅ 1. Clone the Repo

```bash
git clone https://github.com/BharathK05/Intel_Chatbot.git
cd Intel_Chatbot
```

### ✅ 2. Create `.env` File

Open the `.env` file in the root folder:

```
GEMINI_API_KEY=your-google-api-key-here
```

> 🔑 Get your API key from [Google AI Studio](https://makersuite.google.com/app/apikey)

### ✅ 3. Install Dependencies

Make sure Python 3.8+ is installed, then:

```bash
pip install -r requirements.txt
```

If you don’t have a `requirements.txt`, you can install manually:

```bash
pip install google-generativeai python-dotenv transformers torch
```

---

## ▶️ Run the Chatbot

```bash
python integrated_chatbot.py
```

You'll see:

```
🤖 Chatbot Ready!
💬 Every response is exactly one sentence
🔧 Type 'quit' to exit
```

Type your messages and chat with the bot. Type `quit` to end the chat and get your **final mood score**.

---

## 💬 Mood Categories

The chatbot uses a distilled BERT model to classify each user message into one of 27 emotions and maps them into **5 moods**:

| Mood     | Emotions Grouped |
|----------|------------------|
| Happy    | joy, love, amusement, admiration, optimism... |
| Calm     | neutral, realization, curiosity |
| Confused | surprise, confusion, nervousness |
| Sad      | sadness, grief, disappointment |
| Angry    | anger, disgust, fear |

---

## 📊 How Mood Score Works

Each input gets a score (e.g., Happy = 90, Angry = 15), and a final average is calculated at the end:

```
Final Mood Score: 58.33
Dominant Mood: Confused
```

---

## 📁 Folder Structure

```
project/
├── gemini_one_line_chatbot.py     # Main Python chatbot file
├── .env                           # Holds API key
├── README.md
```

---

## 📜 License

MIT License © 2025 Bharath Kalimuthu

---

## 🙌 Acknowledgments

- [Google Generative AI (Gemini)](https://ai.google.dev/)  
- [HuggingFace Transformers](https://huggingface.co/)
