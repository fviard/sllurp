# RFID Reader Control

This project provides a web-based interface to control an RFID reader and manage tag data. It includes a FastAPI backend to handle RFID reader operations and a simple HTML frontend to interact with the backend.

## Features

- **Start RFID Reader**: Initiate the RFID reader to start scanning for tags.
- **Stop RFID Reader**: Stop the RFID reader and return tag data.
- **Get Tags**: Retrieve the list of tags scanned by the RFID reader.
- **Status**: Check the status of the RFID reader (connected, disconnected).
- **State**: Get the state of the RFID reader.

## Package manager

- uv (https://docs.astral.sh/uv/)

## Requirements

- Python 3.13
- FastAPI
- sllurp
- uvicorn
- pydantic
- websockets

## Setup

1. **Clone the repository**:

   ```sh
   git clone <repository-url>
   cd <repository-directory>/examples/fastapi
   ```

2. **Create a virtual environment**:

   ```sh
   python -m venv .venv
   source .venv/bin/activate
   ```

3. **Install dependencies**:

   ```sh
   pip install -r requirements.txt
   ```

## Running the Application

1. **Start the FastAPI server**:

   ```sh
   python app.py
   ```

   ```sh
   uv run app.py
   ```

2. **Open the `index.html` file in your browser** to access the web interface to test.

## API Endpoints

- **GET /start**: Start the RFID reader.
- **GET /last-read**: Get the last scanned tags.
- **GET /stop**: Stop the RFID reader and return tag data.
- **GET /status**: Get the status (connected, disconnected) of the RFID reader.
- **GET /state**: Get the state of the RFID reader.
- **GET /clear**: Clear tag data
