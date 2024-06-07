# Medical Report Extractor

This repository contains a Python project that leverages the LangChain framework and Google's Gemini 1.5 Pro language model to extract structured data from medical lab reports, particularly Complete Blood Count (CBC) reports. The project uses Pydantic for data validation and structured output.

## Features

- **LangChain Integration**: Utilizes LangChain's capabilities for building robust and flexible language model interactions.
- **Gemini 1.5 Pro**: Employs Google's advanced language model with a million-token context window for comprehensive text understanding and generation.
- **Pydantic Models**: Ensures data validation and structured output using Pydantic models.
- **Image Processing**: Processes medical report images to extract and format data into a predefined schema.
- **Safety Settings**: Configures safety settings to filter out harmful content.

 ## Usage
Define the Pydantic models for the CBC report.
Create and configure the LangChain pipeline to process input images and extract data.
Invoke the chain with an image URL to get the structured JSON output.

## Getting Started

### Installation

```bash
pip install langchain
pip install langchain-google-genai
pip install pydantic

## Setup
##Configure the API key for accessing the Gemini 1.5 Pro model.


import os
from google.colab import userdata
api_key = userdata.get('GOOGLE_API_KEY')
os.environ["GOOGLE_API_KEY"] = api_key





