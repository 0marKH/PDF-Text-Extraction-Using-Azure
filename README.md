Azure Form Processing with Python

Overview

This repository contains a Jupyter Notebook for processing PDFs using Azure Form Recognizer. The notebook extracts structured data from PDF documents, specifically focusing on:

Page 1: Extracts total number of cars and revenue.

Page 3: Extracts entry, exit, total counts, and peak utilization data.

The extracted data is cleaned and formatted into Pandas DataFrames for further analysis.

Features

Uses Azure AI Form Recognizer for automated document analysis.

Parses and structures data from PDF tables.

Cleans numeric fields and formats date values.

Supports integration with Pandas and PySpark.

Implements error handling for missing or malformed data.

Requirements

To use this notebook, install the following dependencies:

pip install azure-ai-formrecognizer pandas pyspark

Setup Instructions

Set Up Azure Form Recognizer

Create a Form Recognizer resource in Azure Portal.

Retrieve the endpoint and API key.

Configure Environment Variables

Store your credentials in environment variables:

export AZURE_FORM_RECOGNIZER_ENDPOINT="your_endpoint_here"
export AZURE_FORM_RECOGNIZER_KEY="your_key_here"
export PDF_PATH="path/to/your/pdf"

Run the Notebook

Open Jupyter Notebook and execute the cells to process the document.

File Structure

.
├── azure_form_processing.ipynb  # Main Jupyter Notebook
├── README.md                    # Project Documentation
└── requirements.txt              # Dependencies list (if needed)

Usage

Modify the PDF_PATH variable to point to your document.

Run the notebook to extract and clean the data.

Use the processed DataFrames for further reporting and analysis.

Contributing

Feel free to submit issues or pull requests for improvements.
