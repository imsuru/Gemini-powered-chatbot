# 🤖 Gemini Powered Chatbot (Google Colab)

A simple AI chatbot built using **Google Gemini API**, designed to run entirely in **Google Colab** — no local setup required.

This project demonstrates how to integrate Gemini into a conversational chatbot using Python in a single notebook.

---

## 🚀 Features

* 💬 Interactive AI chatbot
* 🧠 Powered by Google Gemini
* ☁️ Runs fully in Google Colab
* 🔑 Secure API key usage
* 🧪 Beginner-friendly implementation

---

## 📂 Project File

```
Gemini_Chatbot.ipynb
```

This notebook contains:

* Gemini API setup
* API key configuration
* Chat loop logic
* Example prompts

---

## ▶️ How to Run

### 1️⃣ Open in Google Colab

Upload the notebook to Google Colab
OR

Click:

```
https://colab.research.google.com/
```

Then upload `Gemini_Chatbot.ipynb`.

---

### 2️⃣ Install Dependencies (if required)

Inside Colab:

```python
!pip install -q google-generativeai
```

---

### 3️⃣ Add Your Gemini API Key

Get your API key from:
👉 [https://aistudio.google.com/](https://aistudio.google.com/)

Then in Colab:

```python
import os
os.environ["GEMINI_API_KEY"] = "your_api_key_here"
```

Or use:

```python
from google.colab import userdata
```

(for secure storage if configured)

---

### 4️⃣ Run All Cells

Click:

```
Runtime → Run All
```

Start chatting with your Gemini-powered bot 🚀

---

## 💻 Example Code Snippet

```python
import google.generativeai as genai
import os

genai.configure(api_key=os.getenv("GEMINI_API_KEY"))

model = genai.GenerativeModel("gemini-pro")

chat = model.start_chat()

response = chat.send_message("Hello!")
print(response.text)
```

---

## 🛠 Requirements

* Google Account
* Gemini API Key
* Internet connection
* Google Colab

---

## 📌 Use Cases

* Learning Generative AI
* AI Chatbot Prototyping
* NLP Experiments
* Academic Projects

---

## 📜 License

MIT License

---

## ⭐ Support

If you found this helpful, consider giving the repository a ⭐ on GitHub!

---
