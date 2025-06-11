💼 AI Cold Email Generator
An intelligent tool that generates professional, personalized cold emails for job applications. Built with LangChain, ChromaDB, and Hugging Face, it tailors emails using job descriptions and user details to help applicants stand out.

🚀 Key Features
✉️ Generates structured and engaging cold emails

🧠 Uses Hugging Face's Mistral-7B-Instruct model via LangChain

🔎 Retrieves relevant portfolio data using ChromaDB and MiniLM embeddings

🧾 Simple Streamlit-based interface for easy use

🧠 Tech Stack
Tool	Role
Python	Core programming language
Streamlit	UI framework
LangChain	LLM orchestration
HuggingFaceHub	LLM inference (Mistral-7B-Instruct)
ChromaDB	Vector search for portfolio context
MiniLM (HF model)	Local embedding model for text similarity
dotenv	Securely load environment variables

📁 Folder Structure
bash
Copy
Edit
AI-Cold-Email-Generator/
│
├── app.py                # Main Streamlit application
├── .env                  # HuggingFace API token
├── requirements.txt      # Python dependencies
├── all-MiniLM-L6-v2/     # Local model for embeddings
└── README.md             # Project documentation
⚙️ Setup Instructions
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/your-username/AI-Cold-Email-Generator.git
cd AI-Cold-Email-Generator
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Add HuggingFace API Token
Create a .env file in the root folder:

env
Copy
Edit
HUGGINGFACEHUB_API_TOKEN=your_huggingface_token
Or use the provided .env file:

bash
Copy
Edit
cp .env.example .env
4. Start ChromaDB Server
Make sure ChromaDB server is running locally at:

bash
Copy
Edit
localhost:8000
Use:

bash
Copy
Edit
chromadb run
Install ChromaDB with: pip install chromadb

5. Run the Application
bash
Copy
Edit
streamlit run app.py
🧪 How It Works
User inputs a job description.

Fills in their details (name, education, experience, etc.).

App:

Retrieves relevant context from ChromaDB.

Uses Hugging Face's Mistral-7B-Instruct to generate a personalized email.

Email is shown on-screen, ready to copy and send.

📌 Requirements
Python 3.8+

Streamlit

Hugging Face Transformers

LangChain

ChromaDB

PyTorch

All dependencies are listed in requirements.txt.

📌 Future Improvements
🔗 Upload resume and auto-extract details

📝 Multi-template support (internship, freelance, etc.)

🌐 Deploy as a web service

📜 License
This project is licensed under the MIT License.

🙋‍♂️ Author
Gulfam Baig
Email: gulfambaig30@gmail.com

