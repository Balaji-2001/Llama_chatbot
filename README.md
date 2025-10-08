# Llama RESTful Chatbot – Python Flask (Colab Demo)

## Overview

This project implements a RESTful chatbot API using the Llama model and Flask in Python. User messages are accepted via HTTP POST and answered with Llama-generated responses. All code, tests, and troubleshooting are available in a Colab/Jupyter notebook.

***

## Features

- *Llama language model* (via llama-cpp-python)
- *REST API in Flask:* /chat endpoint for POST user messages
- *pyngrok integration* for Colab public demo
- Organized example images:
  - Output_Screenshot/ — Colab API output, chatbot demo screenshots
  - Error_Screenshot/ — Error images (curl, DNS, Colab)
- Professional, clean file/folder organization

***

## Quick Start

### 1. Run in Google Colab

- Open Llama_chatbot.ipynb in Colab
- Install dependencies in the notebook as shown
- Run API demo cell to print your ngrok URL

### 2. Test the API

Send a POST request using curl or Postman:
bash
curl -X POST "http://YOUR_NGROK_HOST/chat" \
     -H "Content-Type: application/json" \
     -d "{\"message\": \"What is Python?\"}"

Replace YOUR_NGROK_HOST with the URL Colab outputs.

***

## Folder Structure



|-------------|
Llama_chatbot/  
├── Output_Screenshot/  |
│   └── example_colab_output.png  |
├── Error_Screenshot/  |
│   └── example_curl_er ror.jpg  |
├── Ngrok_Auth_token  |
├── Llama_chatbot.ipynb  |
├── Llama_chatbot.py  |
├── README.md  |

***

## Screenshots

*API Output Example:*  


*Error Sample:*  

***

## Troubleshooting

- Some curl/networking errors expected with Colab/ngrok—see Error_Screenshot for authentic troubleshooting history.
- Solution and API fully reproducible in Colab for evaluation; setup ready for any future VM/cloud environment.
