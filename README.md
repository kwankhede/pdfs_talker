# PDFs Talker - Chatbot for PDF Documents

PDFs Talker is a Streamlit application that enables users to interactively chat with multiple PDF documents using LangChain and Google Gemini Pro models. This chatbot extracts text from uploaded PDF files, processes them into manageable chunks, and uses AI models to generate conversational responses based on user queries.

![Screenshot](screenshot_panda.png)

## Features

- **Upload PDF Files:** Users can upload multiple PDF files simultaneously.
- **Extract Text:** Automatically extracts text content from uploaded PDFs.
- **Text Chunking:** Splits extracted text into smaller chunks for efficient processing.
- **AI Powered Responses:** Utilizes Google Gemini Pro models to generate intelligent responses based on user questions.
- **Interactive Interface:** Powered by Streamlit, providing a user-friendly and responsive web interface.

## How to Run

### Prerequisites

Ensure you have Python installed on your machine. If not, download and install it from [python.org](https://www.python.org/).

### Installation

1. **Clone the Repository:**

   ```sh
   git clone https://github.com/kwankhede/pdfs_talker.git
   cd pdfs_talker
   ```

2. **Create a Virtual Environment:**

   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install the Required Dependencies:**

   ```sh
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables:**

   - Create a `.env` file in the root directory.
   - Add your Google API key to the `.env` file:

     ```plaintext
     GOOGLE_API_KEY=your_google_api_key
     ```

5. **Run the Streamlit App:**

   ```sh
   streamlit run app.py
   ```

## Dependencies

- **Streamlit**: For building the interactive web interface.
- **PyPDF2**: For reading and extracting text from PDF files.
- **LangChain**: For text splitting and handling language models.
- **Google Generative AI**: For generating embeddings and conversational responses.
- **python-dotenv**: For managing environment variables.
- **FAISS**: For similarity search on text chunks.

## Usage

1. **Upload PDF Files:**

   - Use the sidebar to upload multiple PDF files.

2. **Ask Questions:**

   - Enter your question in the text input field.

3. **View Responses:**

   - The application will display detailed responses based on the content of the uploaded PDFs.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [LangChain](https://github.com/langchain/langchain)
- [Google Generative AI](https://github.com/google/generativeai)
- [Streamlit](https://github.com/streamlit/streamlit)
