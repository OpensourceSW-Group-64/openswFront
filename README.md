# openswFront.html

## Introduction

**`openswFront.html`** is a frontend web page designed to work with a backend **emotion analysis API**. Users can upload an image to the page, which then sends the image to the backend server (`/predict` endpoint) for emotion recognition. The server returns the predicted emotion and confidence score, which are displayed directly on the page.

## Key Features

- **Image Upload**: Easily select an image file from your device.
- **Emotion Prediction**: Automatically sends the uploaded image to the `/predict` endpoint for analysis.
- **Result Display**: Shows the predicted emotion and confidence score returned by the server.
- **Image Preview**: Displays a preview of the selected image before sending it to the server.

## Requirements

### Backend Server

You need a backend service running that can process **POST** requests at the `/predict` endpoint.

For example, a Python-based server (e.g., **Flask**, **FastAPI**, or **Streamlit**) that:  
- Accepts an image file as input  
- Performs emotion analysis on the image  
- Returns a **JSON** response containing the predicted emotion and confidence score

### Web Browser

Use a modern browser like **Chrome**, **Firefox**, or **Edge** for the best experience.

## Usage

1. Start the backend server so that it is accessible (e.g., `http://localhost:5000/predict`).
2. Open **`openswFront.html`** in your web browser.  
   You can open it by double-clicking the file (if security settings allow) or by serving it through a simple HTTP server, such as:

   ```bash
   python -m http.server 8000
