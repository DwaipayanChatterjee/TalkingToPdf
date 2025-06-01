# PDF-MAN Chat App

## Introduction
------------
This MultiPDF Chat App is a Python-based application that enables users to interact with multiple PDF documents through natural language queries. By leveraging a language model, the app generates accurate and contextually relevant responses based on the content of the loaded PDFs. Please note that responses are limited to information contained within the uploaded documents.

## How It Works
------------

![MultiPDF Chat App Diagram](./docs/PDF-LangChain.jpg)

The application operates through the following steps to generate responses to user queries:

1. PDF Loading: It reads and extracts text content from multiple PDF documents.

2. Text Chunking: The extracted text is segmented into manageable chunks for      efficient processing.

3. Embedding Generation: A language model creates vector embeddings for each text chunk, capturing their semantic meaning.

4. Similarity Matching: Upon receiving a user question, the app compares it with the embeddings and retrieves the most semantically relevant chunks.

5. Response Generation: The selected text chunks are passed to the language model, which formulates a response based on the relevant PDF content

## Dependencies and Installation
----------------------------
To install the PDF-MAN Chat App, please follow these steps:

1. Clone the repository to your local machine.

2. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

3. Obtain an API key from OpenAI and add it to the `.env` file in the project directory.
```commandline
OPENAI_API_KEY=your_secrit_api_key
```

## Usage
-----
To use the PDF-MAN Chat App, follow these steps:

1. Ensure that you have installed the required dependencies and added the OpenAI API key to the `.env` file.

2. Run the `main.py` file using the Streamlit CLI. Execute the following command:
   ```
   streamlit run app.py
   ```

3. The application will launch in your default web browser, displaying the user interface.

4. Load multiple PDF documents into the app by following the provided instructions.

5. Ask questions in natural language about the loaded PDFs using the chat interface.