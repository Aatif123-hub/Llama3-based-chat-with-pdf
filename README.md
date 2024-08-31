# Chat with Multiple PDFs using LLaMA 3 🦙

This Streamlit application allows you to interact with multiple PDF documents using the LLaMA 3 model. You can ask questions related to the content of the uploaded PDFs, and the model will provide answers based on the context provided.

## Features

- Upload and process multiple PDF files.
- Extract text from PDF files.
- Use Llama 3 model for question answering based on the content of the PDFs.
- Interact with the processed content using a conversational interface.

## Prerequisites

- Python 3.8 or higher
- Install the required Python packages using `pip` and requirements.txt
- Ensure you have access to the LLaMA 3 model
- To get access to llama3, go to the ollama website and download the model
- Run the model in your terminal to use it in this project

## Installation

1. **Clone the Repository**

   git clone https://github.com/Aatif123-hub/Llama3-based-chat-with-pdf.git

   cd Llama3-based-chat-with-pdf
   
3. **Install the Required Dependencies**

   pip install -r requirements.txt

   you might need to install a few packages which are not mentioned in the requirements file

4. **Add the access tokens to the .env file**

   Add the huggingface token to use the embeddings

    I have not added the openai token because I am not using the chatgpt model

3. **Start the Streamlit Application**

   streamlit run app.py

   Use this command in your terminal to run the project

## Main Components
get_pdf_text(pdf_docs): Extracts text from the uploaded PDF files.

get_text_chunks(text): Splits the extracted text into manageable chunks.

get_vectorstore(text_chunks): Stores the text chunks in a vector database for retrieval.

get_conversation_chain(vectorstore): Initializes the LLaMA 3 model and sets up the conversational chain.

handle_userinput(user_question): Handles user questions and provides answers based on the content of the PDFs.

main(): The main function that sets up the Streamlit interface and orchestrates the flow.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request with your changes.

## License
This project is licensed under the Apache License. See the LICENSE file for more details.
