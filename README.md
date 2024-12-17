# Smart Knowledge Assistant for Healthcare Professionals

## Overview
This project leverages state-of-the-art natural language processing (NLP) tools to create a Smart Knowledge Assistant for healthcare professionals. The system processes medical documents like the GALE OF ENCYCLOPINDIA 3RD EDDITION, stores the information in a vector database, and uses a question-answering interface to retrieve relevant information. It is designed to facilitate quick access to critical medical knowledge using advanced embeddings and language models.

## Features
1. **PDF Parsing and Text Splitting**
   - Utilizes PyMuPDF to load and split medical documents into manageable chunks for processing.
   - Customizable text splitting using the RecursiveCharacterTextSplitter for optimal chunk sizes and overlaps.

2. **Vector Database Creation**
   - Embeds the document chunks using Google Generative AI Embeddings.
   - Stores the embeddings in a Chroma vector database for efficient similarity-based retrieval.

3. **Question-Answering System**
   - Supports question-answering using a retrieval-augmented generation (RAG) pipeline.
   - Allows dynamic interaction through a loop for continuous querying.

4. **Integration with Google Generative AI**
   - Uses Google Gemini models for both embeddings and conversational responses.
   - Features a system prompt for concise and context-aware answers.

5. **Export Capabilities**
   - Downloads the vector database for local usage.

## Prerequisites
- Google Colab environment
- Python 3.7+
- Google Generative AI API key

## Installation
1. Open the provided `.ipynb` file in Google Colab.
2. Install the required dependencies by running the relevant cells in the notebook. Dependencies include:
   - `pymupdf`
   - `langchain`
   - `langchain_community`
   - `langchain-google-genai`
   - `chromadb`

## Usage Instructions

### Step 1: Setup
- **Mount Google Drive**: Ensure your files are accessible by mounting Google Drive.
- **Load PDF**: Use the provided notebook to load your PDF file into the system.

### Step 2: Preprocess Data
- Split the document into smaller chunks for efficient processing.

### Step 3: Create Vector Database
- Embed the processed text using Google Generative AI embeddings.
- Store the embeddings in a Chroma vector database.

### Step 4: Querying
- Use the notebook to set up a retriever and query the vector database with questions.

### Step 5: Interactive QA
- Engage with the question-answering system by asking medical queries. The assistant will provide concise, context-aware responses.

### Step 6: Export Database
- Export the vector database as a zip file for local use if required.

## Running the Notebook
1. Open the `.ipynb` file in Google Colab.
2. Run each cell sequentially to:
   - Set up the environment.
   - Process the medical document.
   - Query the system with medical-related questions.
   - Export results as needed.

## Limitations
- Requires a valid Google Generative AI API key.
- Designed for single-file processing; handling multiple files may need adjustments.
- Requires an active internet connection for API calls.

## Future Enhancements
- Add support for additional document formats.
- Deploy the system as a standalone web application for broader accessibility.
- Optimize for handling larger datasets seamlessly.


