**Created by:** Afifa Siddique during the internship at Pakistan International Airlines (PIA).

**PIA** is the national flag carrier of Pakistan, providing domestic and international air travel services. The organization also maintains a dedicated medical division to support the health and well-being of its employees and their families. 

---
#### Disclaimer:
These two projects are solely the property of **Pakistan International Airlines (PIA)** and are not permitted for use, distribution, or reproduction by any other individual or entity.

---

# PROJECT : 01 AI-powered Customer Support Chatbot 

This is a customer support chatbot developed for Pakistan International Airlines (PIA) as part of an internship project. The chatbot is designed to assist users by providing answers to frequently asked questions about PIA’s services.

---

##  Use Cases

-  Flight bookings & schedules  
-  Baggage policies  
-  Refunds & cancellations  
-  Medical/travel assistance  
-  Contact information  
-  International destinations  

The chatbot is powered by locally stored PDF documents and uses Retrieval-Augmented Generation (RAG) with a Groq-hosted LLaMA3 model for fast and accurate answers.

---

##  Tech Stack

| Tool         | Purpose                                      |
|--------------|----------------------------------------------|
| Python 3.11  | Core programming language                    |
| Hugging Face | Local embedding models (e.g., BAAI/bge-small-en) |
| LlamaIndex   | PDF ingestion, embedding, and indexing       |
| Groq API     | LLM-powered response generation (LLaMA3)     |
| FastAPI      | Building and hosting RESTful API             |
| Faiss        | Vector store for fast retrieval              |
| HTML         | Output formatting in browser                 |
| VS Code      | Development environment                      |

---

##  How It Works

1. PDF files are stored in the `PIA_KnowledgeBase/` folder.
2. These files are loaded and embedded using `load_and_embed.py`.
3. The index is saved locally in the `index/` folder.
4. FastAPI serves a REST endpoint (`/chat`) that takes a question and returns an answer.
5. The Groq-hosted LLaMA3 model is used to generate natural language answers based on retrieved content.

---

##  Project Structure

PIA_CHATBOT/
├── main.py # FastAPI application

├── load_and_embed.py # Script to process and index PDFs

├── chat_with_groq.py # CLI script for local testing

├── index/ # Vector store index data

├── PIA_KnowledgeBase/ # All PDF documents

├── requirements.txt # Python dependencies

└── README.md # Project documentation

---

#  PROJECT : 02 Medical Data Analytics Report - PIA

Using a combination of **Power BI** and **Python**, we developed an interactive, 8-page dashboard that integrates 10 tables (1 master + 9 reference) to explore:

- Patient visits and diagnostic activity  
- Prescription and medicine utilization  
- Hospitalizations and referrals  
- Certificate issuance patterns  
- Anomaly detection and operational trends

---

##  Key Features

###  Use Case 1: Medicine Abuse Detection
- Identifies patients receiving unusually high quantities of specific medicines
- Helps flag potential overuse or overprescription

###  Use Case 2: Frequent Patient Detection
- Highlights patients with high visit frequency in a short time
- Useful for spotting chronic conditions or administrative misuse

###  Additional Visual Insights
- Internal vs external lab test trends  
- Referral tracking to external specialists  
- Hospital admission patterns by city  
- Certificate (Fitness & Medical) issuance trends  
- Prescription load by dispensary/location

---

##  Tools & Technologies
- **Power BI** (Data Modeling, DAX, Visualization)
- **Python** (Preprocessing)
- **Excel** (Data review and cleanup)

---

##  Data Overview
- 1 Master Table: Patient assignment records  
- 9 Reference Tables: Lab tests, prescriptions, hospitalizations, referrals, certificates, locations, etc.

---

## Key Outcomes
- Delivered a fully interactive report to PIA’s medical division  
- Improved operational transparency using data-driven dashboards  
- Built end-to-end reporting from raw data to strategic insights

---
