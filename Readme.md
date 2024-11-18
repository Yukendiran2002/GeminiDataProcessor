# GeminiDataProcessor

## Overview

`GeminiDataProcessor` is a Python library that streamlines data processing through the use of Google's generative AI models (Gemini). It allows users to generate structured responses for tabular datasets using customizable prompts and schemas.

## Features

- **Integration with Gemini AI**: Process data through Google's generative AI models.
- **Asynchronous Processing**: Supports efficient handling of large datasets using `asyncio`.
- **Flexible Schema**: Define custom output schemas for structured JSON responses.
- **Error Handling**: Robust error management for API and data parsing issues.
- **Progress Tracking**: Real-time processing feedback with `tqdm`.

## Installation

You can install the module using pip:

```bash
pip install gemini_data_processor
```

```python
from gemini_batch_processor import GeminiBot

bot = GeminiBot(
    input_file="input_data.csv",
    prompt_template="Generate a summary for: {row[column name]}",
    key_names="summary,details",
    api_key="your_google_api_key",
    model="gemini-1.5-flash-002"
)
```
```python
from gemini_batch_processor import GeminiBot
GeminiBot.model_list(api_key="your_api_key")
```