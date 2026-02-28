AI Digital Twin: Personal Career Assistant
This repository contains the source code for an AI Digital Twin, a personalized conversational agent designed to represent your professional persona. By leveraging Large Language Models (LLMs) and document processing, this tool transforms a static PDF resume into an interactive, 24/7 professional assistant.

🚀 Project Overview
The AI Digital Twin acts as an automated extension of your LinkedIn profile. It allows recruiters, collaborators, and visitors to interact with your "career brain" in real-time, asking questions about your experience, skills, and projects without requiring manual intervention.

🛠️ The Tech Stack
Language: Python 3.x

PDF Intelligence: PyPDF for robust text extraction from complex resume layouts.

Core Logic: OpenAI GPT-4o-mini for high-speed, cost-effective natural language reasoning.

Interface: Gradio for a clean, responsive web UI that can be deployed instantly.

Deployment: Optimized for Hugging Face Spaces using gradio deploy.

✨ Key Features
Automated Data Ingestion: No hard-coding required. The system reads your latest PDF resume and updates its knowledge base instantly.

Persona Grounding: Uses advanced System Prompting to ensure the AI speaks in a professional, helpful, and accurate tone consistent with your brand.

Context-Aware Chat: Responds to specific queries about technologies (e.g., Python, Unreal Engine 5) or specific roles based on the uploaded data.

Zero-Maintenance Hosting: Designed for permanent, free hosting with easy GPU upgrade paths.

📖 How It Works
Extraction: The script utilizes PyPDF to parse and clean text from your professional documents.

Context Construction: The extracted text is injected into a "System Role" message, providing the GPT-4o-mini model with a permanent frame of reference.

Interaction: Users enter questions via the Gradio interface; the model references your resume data to provide accurate, "first-person" responses.

🛠️ Installation & Setup
Clone the Repository:

Bash
git clone https://github.com/yourusername/ai-digital-twin.git
cd ai-digital-twin
Install Dependencies:

Bash
pip install -r requirements.txt
Set Up API Key: Create a .env file and add your OpenAI key:

Bash
OPENAI_API_KEY=your_actual_key_here
Run Locally:

Bash
python app.py
📈 Future Roadmap
RAG Integration: Moving from basic prompting to a Vector Database (like Pinecone or FAISS) for handling multiple documents.

Multi-Modal Support: Allowing the twin to explain projects using images or video links.

Analytics Dashboard: Tracking what questions visitors ask most frequently.