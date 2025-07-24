## Locally run RAG with Llama 3.1 and Ollama

### Prerequisites
Python 3.8+Ollama

### How to Run:

Install Ollama Models
Ensure the Ollama application is running, then pull the required models from your terminal.

ollama pull llama3.1
ollama pull nomic-embed-text

### Set Up Python Environment

Create and activate a virtual environment in your project directory.

Create the environment
python3 -m venv venv

Activate the environment (macOS/Linux)
source venv/bin/activate

### Install Dependencies
Install the required Python libraries.

pip install langchain langchain-community langchain-text-splitters langchain-ollama pypdf faiss-cpu ollama jupyter
### Add Your Document

Create a data folder in the project directory.
Place your PDF inside the data folder.In test.ipynb, update the file_path variable to point to your PDF.file_path = "data/your_document_name.pdf"

### Launch and Run
Start the Jupyter server from your terminal:

jupyter notebook

Open test.ipynb in your browser.
Run the cells sequentially (Shift + Enter) to load the document and ask questions.

### Next steps
Find a more robust prompt augmenting template
Support Multiple Documents uploads
Move towards chatbot from single querries
Explore math behind embedded vector database
