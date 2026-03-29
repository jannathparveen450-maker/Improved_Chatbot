# 🤖 Gemini Chatbot using Streamlit

This project is a simple and interactive AI chatbot built using **Streamlit** and **Google Gemini API**. It allows users to have real-time conversations with an AI model while maintaining chat history within the session.



## Features

*  Real-time chat interface
*  Powered by Google Gemini (gemini-2.5-flash)
*  Maintains conversation history (session-based)
*  Clean and simple UI using Streamlit
*  Secure API key handling using `.env`



##  Tech Stack

* Python
* Streamlit
* Google Generative AI (Gemini API)
* python-dotenv



##  Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/jannathparveen450-maker/Improved_Chatbot
cd Improved_Chatbot
```


### 2️⃣ Create virtual environment (recommended)

```bash
python -m venv myenv
myenv\Scripts\activate   # Windows
```


### 3️⃣ Add API Key

Create a `.env` file in the root folder and add:

```
GOOGLE_API_KEY=your_api_key_here
```

### 4️⃣ Run the app

```bash
streamlit run app.py
```

## 🧠 How It Works

* The app uses **Streamlit** to create a chat UI.
* User messages are sent to the **Gemini model** using:

  ```python
  model.start_chat()
  ```
* Chat history is stored in:

  ```python
  st.session_state
  ```
* Responses are generated and displayed in real time.


##  Role Handling

Since Streamlit and Gemini use different role names:

* `"model"` → `"assistant"`
* `"user"` → `"user"`

A helper function is used to convert roles for display.

##  Author

**Jannath Parveen**

If you like this project, give it a ⭐ on GitHub!
