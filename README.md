# Cooking Assistant Chatbot

A comprehensive web application for suggesting recipes, answering culinary questions, and helping you cook creatively with what you already have in your kitchen.

## Installation

1. Clone the repository: `git clone https://github.com/IamHoa05/cooking-assistant-chatbot.git`
2. Navigate to the directory: `cd cooking-assistant-chatbot`
3. Get API Key: Visit https://groq.com/, log in with your Google account to get a free API Key, then navigate to the app directory and create a `.env` file with `GROQ_API_KEY="Your_Copied_API_Key"` (e.g., GROQ_API_KEY=abshgsksfkslgjsl)
4. Install libraries: `cd backend` then `pip install -r requirements.txt`
5. Navigate to `backend/app/utils` and run: `python build_embedding.py`, `python build_faiss_index.py`, `python build_intent_embedding.py`
6. Navigate back to the `backend` directory and run: `uvicorn main:app --reload`

---

# Group Assignment Report - Introduction to Artificial Intelligence

**Information:** Course: MAT3508 - Introduction to Artificial Intelligence | Semester: Semester 1 - 2025-2026 | University: VNU-HUS (Vietnam National University, Hanoi - University of Science) | Title: Cooking Assistant Chatbot | Submission Date: November 30, 2025 | PDF Report: 📄 [Link to PDF report in this repository] | Presentation Slides: 🖥️ [Link to presentation slides in this repository] | Repository: 📁 Includes source code, data, and documentation (or external links if needed)

**Group Members:** Nguyễn Thị Hòa (23001521, IamHoa05) - Team Leader, Backend, NLP; Đào Thị Ngọc Bích (23001501, daobich14) - Frontend, Data Preprocessing; Đinh Thị Kiều Na (23001537, kieuna2005) - Frontend, Embedding; Dương Diễm Quỳnh (23001555, ddquynh) - Backend, LLM; Lưu Thị Thủy Tiên (23001563, ttien2312) - Backend, NLP

## Report Structure Overview

### Chapter 1: Introduction

**Project Summary:** The Cooking Assistant Chatbot project is built to develop an intelligent virtual assistant in the culinary domain. The chatbot helps users search for dishes based on available ingredients, provides detailed easy-to-understand cooking instructions, and suggests cooking tips, nutritional notes, and cooking time. The system is designed to understand natural language, process structured recipe data, and provide recommendations suitable for users' tastes, preferences, and actual kitchen conditions.

**Problem Statement:** In the context of increasing home cooking demand, especially following recent social changes, many people want to cook at home to save costs, ensure health, and improve cooking skills. However, finding suitable recipes with available ingredients or time constraints remains a challenge. The project aims to create a cooking chatbot that understands users by recognizing requests, preferences, and dietary restrictions; provides intelligent recipe suggestions by combining rich recipe data with natural language processing capabilities; and offers friendly interaction to deliver a personalized, intuitive, and easy-to-use experience.

### Chapter 2: Methodology & Implementation

**Methodology:** Natural Language Processing uses tokenization, embedding, and semantic search techniques to understand user questions. The Recipe Database standardizes data from multiple sources, storing attributes such as ingredients, cooking time, difficulty level, serving size, and nutritional information. The Recommendation Model combines LLM with content-based search algorithms to provide suitable recipe suggestions. The Intelligent Recommendation Algorithm filters by ingredients, dish type, cooking time, and customizes according to personal preferences.

**Implementation:** Frontend is a user-friendly Web interface. Backend provides API for managing recipe data, receiving and processing requests from frontend. Tools and Frameworks include Python, Hugging Face Transformers for NLP, FAISS for similarity search, and Groq for LLM integration.

### Chapter 3: Results & Analysis

**Results & Discussion:** Recommendation Accuracy: The system can provide suitable recipes for over 85% of user test requests. Response Time: Average under 5 seconds per request. User Feedback: 90% of testers rated the experience as easy to use, and 80% found recipe suggestions matched their available ingredients. Analysis: Combining NLP with structured recipe data helps the system understand context and provide more accurate recommendations compared to keyword-based chatbots.

### Chapter 4: Conclusion

**Conclusion & Future Development:** Conclusion: The project has successfully developed a cooking chatbot capable of understanding natural language, providing intelligent recipe suggestions, and offering detailed cooking guidance. It helps users save time, reduce ingredient waste, and enhance their cooking experience. Future Development: Integrate advanced machine learning for personalized recommendations based on eating habits; support multiple languages and voice recognition; develop a mobile app to increase user accessibility.

### References & Appendix

**References:** FAISS: Facebook AI Similarity Search (https://faiss.ai/); FAISS Tutorial (https://www.datacamp.com/blog/faiss-facebook-ai-similarity-search); HuggingFace Course – FAISS (https://huggingface.co/learn/llm-course/vi/chapter5/6); ChatGroq – LangChain Documentation (https://docs.langchain.com/oss/python/integrations/chat/groq); ChatGroq – LangChain Messages (https://docs.langchain.com/oss/python/langchain/messages)

## Submission Checklist

- [X] Complete detailed PDF report following the above structure
- [X] Adhere to format and content as instructed by the lecturer
- [X] Add project-specific sections if needed
- [X] Check grammar, expression, and technical accuracy
- [X] Upload PDF report, presentation slides, and source code
- [X] Ensure all source code is fully documented with comments and docstrings
- [X] Verify all links and references work correctly
