# Legal Document Summarization | Python, NLP, Transformers, Gradio
**November 2023**

This project involves developing an NLP-based legal document summarization system using both extractive and abstractive summarization techniques. The system leverages transformer models (specifically BART) to generate concise and informative summaries while preserving essential legal details. A Gradio-based user interface is built to showcase the summarization system, enabling real-time user interactions with legal case documents.

## Dataset Sources:
1. **IN-Abs**: Indian Supreme Court cases with abstractive summaries.
2. **IN-Ext**: Extractive summaries created by legal experts.
3. **UK-Abs**: U.K. Supreme Court cases with abstractive summaries.

You can access the datasets at the following link:  
[Zenodo Dataset Link](https://zenodo.org/records/7152317)

## Data Split:
- **Training**: 2000 samples
- **Validation**: 2000 samples

## Model: HuggingFace BART Model
- **Pretrained transformer**: Specifically designed for summarization tasks.
- **Encoder-decoder architecture**: Suitable for generating both extractive and abstractive summaries.

## Tokenizer:
- Converts input text into token IDs for compatibility with the transformer model.
- Fine-tuned on domain-specific legal text data to improve summarization performance.

## Workflow:
1. **Load and preprocess legal documents and summaries**.
2. **Tokenization**: Use HuggingFace tokenizer to convert legal text into input IDs for the model.
3. **Fine-tuning**: Fine-tune the pretrained BART model on the training dataset.
4. **Validation**: Evaluate the model on the validation dataset.
5. **Deployment**: Build a Gradio-based UI to allow real-time legal document summarization by users.

## Requirements:
- Python 3.x
- HuggingFace Transformers library
- Gradio
- TensorFlow/PyTorch

