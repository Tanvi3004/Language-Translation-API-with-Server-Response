# Language Translation API with Server Response

This project demonstrates a simple API for language translation. It accepts a text input in one language and returns the translated text in another language. The server response includes metadata and a unique run ID for tracking purposes.

## Features

- **Language Translation**: Translates text from one language to another.
- **API Endpoint**: Accepts POST requests with JSON payload.
- **Server Response**: Returns translated text along with metadata.

## How It Works

1. You send a request to the server with the text you want to translate and the target language.
2. The server processes the request and sends back the translated text.

## Example

### Request

- **URL**: `http://127.0.0.1:8000/chat/invoke`
- **Method**: `POST`
- **Headers**:
  - `accept: application/json`
  - `Content-Type: application/json`
- **Body**: Include the text and target language.

### Response

- **Status Code**: `200` (Success)
- **Response Body**: The translated text and some metadata (like a unique ID for the request).

## Screenshot

Here’s an example of what the server response looks like:

<img width="1440" alt="Image" src="https://github.com/user-attachments/assets/b03ba5af-519c-419e-8997-ae5fab90ae0b" />

## Requirements
  - To run this project, you need the following dependencies:
1. **Python 3.8+**
2. **FastAPI**
3. **Uvicorn**

## Installation
  - Clone the repository:
```bash
git clone https://github.com/Tanvi3004/Language-Translation-API-with-Server-Response.git
cd Language-Translation-API-with-Server-Response
```
 - Install the required dependencies:
```bash
pip install -r requirements.txt
```
 - Run the server:
```bash
python serve.py
```
 - Access the API at 
http://127.0.0.1:8000/docs

### requirements.txt

```plaintext
fastapi==0.95.2
uvicorn==0.22.0
streamlit
fastapi
uvicorn
"langserve[all]"
langchain_core
angchain-groq
langchain
