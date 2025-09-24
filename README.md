# 🔍 LectureLens – RAG based AI teaching assistant  

**LectureLens** is an AI-powered Teaching Assistant that transforms lecture videos into an **interactive Q&A system** using **Retrieval-Augmented Generation (RAG)**.  

Instead of scrubbing through hours of video, students can simply **ask a question** and get a **precise, human-like answer** grounded in the lecture content.  

-----------------------------

## 🌟 Overview 
- Designed and implemented the **end-to-end pipeline** (video → audio → text → embeddings → LLM answers).  
- Integrated **Whisper, bgem3 embeddings, cosine similarity, and LLaMA 3.2** for accurate retrieval and generation.  
- Built a **scalable framework** that can handle multiple lectures and courses.  

-----------------------------

## 💡 Problem Solved  
- 📹 **Lecture videos are long and hard to search** → Students waste time scrubbing through content.  
- 🤔 **Difficult to recall where topics are explained** → Frustrating during revision.  
- 🎯 **Solution**: LectureLens makes lectures **searchable, interactive, and accessible**.  

-----------------------------

## 🔄 Workflow  

1. **Video → MP3** – Extract audio from lecture videos.  
2. **MP3 → JSON** – Transcribe audio into structured text using Whisper.  
3. **JSON → Embeddings** – Convert transcripts into semantic embeddings.  
4. **Query Embedding** – Encode user questions into embeddings.  
5. **Cosine Similarity Search** – Retrieve the most relevant lecture segments.  
6. **Answer Generation** – Generate context-aware answers using LLaMA 3.2.  

-----------------------------

## Demo
>
![WhatsApp Image 2025-09-24 at 12 48 30](https://github.com/user-attachments/assets/5db716de-0c18-4013-833b-3f2a0cfdf92b)
![WhatsApp Image 2025-09-24 at 12 48 33](https://github.com/user-attachments/assets/4d447796-8313-47ea-9344-480cf8073218)
>
![WhatsApp Image 2025-09-24 at 12 48 33 (1)](https://github.com/user-attachments/assets/423b221b-e06b-4abb-a79c-18158cf92b62)
![WhatsApp Image 2025-09-24 at 12 48 33 (2)](https://github.com/user-attachments/assets/8aa53bcd-7f04-473f-a0a1-7866f77f85c6)


------------------------------

## 🧑‍🏫 How to Use LectureLens on Your Own Data  

### Step 1 - Collect your videos
Move all your video files to the videos folder

### Step 2 - Convert to mp3
Convert all the video files to mp3 by ruunning video_to_mp3

### Step 3 - Convert mp3 to json 
Convert all the mp3 files to json by ruunning mp3_to_json

### Step 4 - Convert the json files to Vectors
Use the file preprocess_json to convert the json files to a dataframe with Embeddings and save it as a joblib pickle

### Step 5 - Prompt generation and feeding to LLM
Read the joblib file and load it into the memory. Then create a relevant prompt as per the user query and feed it to the LLM

-------------------------------

## 🛠️ Tech Stack
- **Whisper** – speech-to-text transcription  
- **bgem3 + LLaMA embeddings** – semantic representation  
- **Cosine similarity** – retrieval mechanism  
- **LLaMA 3.2** – large language model for answer generation  
- **Python** – orchestration of the pipeline  

--------------------------------

## 📈 Impact
- ⏱️ Reduced hours of manual video searching to **seconds**  
- 🎓 Enabled **personalized learning** with instant answers  
- 🔎 Showcased how **RAG + LLMs** can make education **smarter and scalable**  
