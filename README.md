# Deep Learning Text Summarization Project

This project focuses on text summarization using deep learning techniques. It includes two main components: data preprocessing and text summarization using the BART (Bidirectional and Auto-Regressive Transformers) model.

## Overview

The project consists of the following files:

1. **clean.ipynb**: This Jupyter Notebook contains the code for preprocessing the input data. It removes non-English text and empty rows from the input CSV file. The `is_english` function detects English text using the `langdetect` library, and the `remove_non_english_and_empty_rows` function cleans the input data accordingly.

2. **main.py**: This Python script performs text summarization on the preprocessed data using the BART model. It reads the preprocessed CSV file, generates summaries for each text entry, and writes the summaries back to the CSV file.

## Usage

1. **Data Preprocessing**: Run the `clean.ipynb` notebook to preprocess the input data. Ensure that the input CSV file (`input.csv`) is in the same directory as the notebook. After preprocessing, the cleaned data will be saved to an output CSV file (`output.csv`).

2. **Text Summarization**: Execute the `main.py` script to generate summaries for the preprocessed data. Make sure to specify the input CSV file path (`input_csv_path`) and the output CSV file path (`output_csv_path`). The script utilizes the BART model from the Hugging Face Transformers library to generate summaries.

## Dependencies

- Python 3.x
- Jupyter Notebook (for running `clean.ipynb`)
- Hugging Face Transformers library

## Contributors

- Surendran Venkataraman

## License

This project is licensed under the [MIT License](LICENSE).
