# AI-RAG-AGENT-WITH-REASONING
🧐 Agentic RAG with Reasoning
This is a Streamlit application that demonstrates an intelligent AI agent built with the Agno framework. The agent is a powerful Retrieval-Augmented Generation (RAG) system that goes beyond simple information retrieval by incorporating step-by-step reasoning.

The app allows you to interact with an AI agent that:

Retrieves relevant information from a knowledge base of URLs.

Reasons through the retrieved data to formulate a precise answer.

Answers your questions with citations to its sources.

🚀 How to Run the App
Clone the repository and navigate to the project directory:

Bash

git clone <repository_url>
cd <project_directory>
Create a virtual environment and install dependencies:

Bash

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
pip install -r requirements.txt
Set up your API keys:

Create a file named .env in the root of the project.

Add your Anthropic and OpenAI API keys to the file.

ANTHROPIC_API_KEY="your_anthropic_api_key"
OPENAI_API_KEY="your_openai_api_key"
Run the Streamlit application:

Bash

streamlit run app.py
A new browser tab will open with the application.

⚙️ Key Components
The application is built on a few core technologies that work together to provide its capabilities:

Agno Agent: The central orchestrator that manages the entire process. It uses the ReasoningTools to think through a problem and decide when to retrieve information from the knowledge base.

Knowledge Base (UrlKnowledge): This component ingests text data from a list of URLs and prepares it for retrieval. The default knowledge source is the Agno documentation.

Vector Database (LanceDb): An efficient database that stores the documents' content in a format that allows for fast and accurate semantic search based on the meaning of the text.

Embeddings (OpenAIEmbedder): Used to convert the raw text from the URLs into numerical vectors. This process, called embedding, is what allows the vector database to perform semantic similarity searches.

Large Language Model (Claude): The AI model that powers the agent's reasoning and generation capabilities. It processes the user's query and the retrieved information to produce the final answer.

Streamlit: The framework used to create the user-friendly web interface, which includes interactive elements for API keys, adding new URLs, and displaying the live-streamed reasoning and answers.












Tools

