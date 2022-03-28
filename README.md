# 📚 InsightSummarizer: Unlock Core Insights Effortlessly

**InsightSummarizer** is an AI-powered text summarization tool that condenses lengthy documents into concise, easy-to-digest summaries. Whether you're dealing with books, articles, or reports, **InsightSummarizer** helps you grasp the essential points quickly, saving you time and enhancing understanding.

## Features

- **Chapter-wise Summarization**: Generate summaries for individual chapters, focusing on specific sections of interest.
- **Entire Document Summarization**: Summarize the whole content when documents lack clear divisions.
- **Advanced Natural Language Processing (NLP)**: Powered by cutting-edge NLP techniques to intelligently extract the most relevant information.
- **User-Friendly Interface**: An intuitive interface makes the summarization process seamless for users of all technical backgrounds.
- **Email Notifications**: Receive summarized content directly in your inbox for convenience.

## How It Works

**InsightSummarizer** leverages the **T5-small** pretrained model from HuggingFace Transformers to generate accurate and coherent summaries. The process involves:

1. **Text Segmentation**: The document is divided into chunks, either by chapters or as a whole.
2. **Tokenization**: Chunks are tokenized using **T5Tokenizer** for compatibility with the **T5** model.
3. **Summary Generation**: The tokenized text is processed by the **T5ForConditionalGeneration** model to produce summary token IDs.
4. **Decoding**: Summary tokens are decoded back into human-readable text using the **T5Tokenizer**'s `decode()` function.

## Getting Started

### Prerequisites

- Python 3.x
- Required Python packages listed in `requirements.txt`

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/zjnbwxq/InsightSummarizer.git
   ```

2. **Navigate to the Project Directory**

   ```bash
   cd InsightSummarizer
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

### Usage

#### Command-Line Interface (CLI)

Run **InsightSummarizer** via CLI:

```bash
python3 summarizer_cli.py --path <path-to-your-document>
```

#### Web Interface with Flask

1. **Configure Email Settings**

   Update `sender_address` and `sender_pass` in `mail.py` with your email credentials.

2. **Start the Flask Server**

   ```bash
   python3 app.py
   ```

3. **Access the Web Application**

   Open your browser and navigate to `http://localhost:5000`.

## Contributing

Contributions are welcome! If you'd like to enhance **InsightSummarizer**, please submit a pull request or open an issue. Your feedback and support are greatly appreciated.

## License

**InsightSummarizer** is released under the [MIT License](https://github.com/zjnbwxq/InsightSummarizer/blob/master/LICENSE).

---

*Made by [Xiaoqi Weng](https://github.com/zjnbwxq) from Birmingham with Love❤️*
