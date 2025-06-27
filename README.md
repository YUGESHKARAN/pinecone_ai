# 🤖 Pinecone AI Conversational Chatbot

## 📝 Overview

This project is a conversational chatbot integrated with the Pinecone vector database. Uploaded documents are stored as embeddings with a dimensionality of 384, enabling efficient and intelligent retrieval of information during conversational interactions.

The primary goal of this project is to enhance AI knowledge by allowing the integration of necessary data in the form of documents. This enables the chatbot to perform any kind of domain-specific task by leveraging document-based knowledge, rather than relying on fine-tuning or training the model with new datasets. The repository is focused solely on enabling users to have conversations with the AI based on the knowledge provided.

> **Note:** The knowledge feeding and document upload functionality is implemented in a separate repository: [ai_knowledge](https://github.com/YUGESHKARAN/ai_knowledge.git). This repository is dedicated to the conversational aspect only.

## ✨ Features

- 🗣️ **Conversational AI**: Interacts naturally with users to answer questions and provide information.
- 🌲 **Pinecone Integration**: Connects directly to Pinecone for fast and scalable vector search.
- 🧬 **Document Embeddings**: Stores uploaded documents as 384-dimensional embeddings, supporting accurate semantic search.
- 🎯 **Domain-Specific Knowledge**: Enables AI to answer questions on any topic by connecting to relevant document embeddings.
- ⚡ **Simple Setup**: Easily install and run locally with minimal dependencies.

## 🚀 Getting Started

### ✅ Prerequisites

- 🐍 Python 3.8+
- 🔑 Pinecone account and API key

### 🔐 Required Environment Variables

Create a `.env` file in the root directory and add the following keys:
```env
GROQ_API_KEY=your_groq_api_key
PINECONE_API_KEY=your_pinecone_api_key
```

### 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/YUGESHKARAN/pinecone_ai.git
   cd pinecone_ai
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure Environment Variables:**
   - Set your Pinecone and GROQ API keys as described above or as specified in your deployment setup.

### ▶️ Running the Application

```bash
python index.py
```

## 🗂️ Project Structure

- `index.py`: Main application file.
- `requirements.txt`: Python dependencies.
- `.gitignore`: Git ignored files.

## ⚙️ How It Works

1. **Document Knowledge Feed**: Knowledge integration and document upload is managed via [ai_knowledge](https://github.com/YUGESHKARAN/ai_knowledge.git).
2. **Embedding Generation**: Each document is converted into a 384-dimensional embedding and stored in Pinecone.
3. **Conversational Retrieval**: When queried, the chatbot retrieves the most relevant information based on vector similarity from the stored document embeddings.
4. **Conversation Only**: This repository enables users to perform conversations. Knowledge upload must be handled through the linked knowledge feed repository.

## 🛠️ Technologies Used

- 🐍 Python
- 🌲 Pinecone Vector Database

## 🤝 Contributing

Contributions are welcome! Open an issue or submit a pull request for improvements or bug fixes.

## 📄 License

This project is licensed under the MIT License.

## 📬 Contact

For questions or support, please contact [YUGESHKARAN](https://github.com/YUGESHKARAN).

---

> **Note:** This project is in active development. Features and documentation may change.
