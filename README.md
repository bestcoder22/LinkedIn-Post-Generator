# LinkedIn Post Generator (GenAI Project)

This project is an end-to-end **Generative AI-based tool** that helps LinkedIn influencers create new posts matching their unique writing style.

The tool analyzes an influencer’s previous LinkedIn posts to understand their **tone, topics, structure, and style**, and then uses this insight to generate new posts automatically.

---

## 🧠 Project Overview

Let’s say **Mohan** is a LinkedIn influencer who frequently writes about tech, startups, and personal growth.  
He can upload his **past LinkedIn posts** into this tool, which will:

1. **Analyze** his existing posts and extract key attributes like *topic, length, and language*.
2. Allow him to **select** desired parameters (topic, tone, language, and post length).
3. **Generate** a new post using his past content as examples — ensuring it matches his unique writing style.

---

## ⚙️ Technical Architecture

![Architecture](resources/architecture.jpg)

The system operates in two stages:

1. **Stage 1 – Data Extraction:**  
   Collects past LinkedIn posts and extracts metadata such as topic, language, and length.

2. **Stage 2 – Post Generation:**  
   Uses the extracted parameters and related old posts to guide a **few-shot learning** prompt that helps the **LLM (Llama 3.2)** generate a new post similar to the influencer’s writing style.

---

## 🧩 Technologies Used

- **Llama 3.2** – Open-source Large Language Model for text generation  
- **LangChain** – For prompt management and orchestration  
- **Streamlit** – Interactive web interface for the user  
- **Groq Cloud** – To efficiently run and serve the LLM  
- **Python** – Core programming language  

---

## 🚀 Setup Instructions

1. **Get your API Key**  
   - Go to [Groq Console](https://console.groq.com/keys)  
   - Create a new API key and update it in your `.env` file as:  
     ```bash
     GROQ_API_KEY=your_api_key_here
     ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt

3. **Run the application**  
   ```bash
   streamlit run main.py

## 🖼️ Tool Interface

The interface provides options to:
1.Upload old LinkedIn posts
2.Select post topic, tone, and length
3.Generate new posts instantly in your own writing style

## 🙏 Thank You

Thank you for exploring this project!
