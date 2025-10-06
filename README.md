# FastAPI CICD Learning App

A simple FastAPI application designed to learn Continuous Integration and Continuous Deployment (CI/CD) practices.

## Features

- Simple FastAPI web application
- HTML response with a beautiful UI
- Health check endpoint
- Ready for CI/CD pipeline integration

## Setup with Virtual Environment

### Windows

1. **Run the setup script:**
   ```bash
   setup.bat
   ```

2. **Or manually:**
   ```bash
   # Create virtual environment
   python -m venv venv
   
   # Activate virtual environment
   venv\Scripts\activate.bat
   
   # Install dependencies
   pip install -r requirements.txt
   ```

### Linux/macOS

1. **Run the setup script:**
   ```bash
   chmod +x setup.sh
   ./setup.sh
   ```

2. **Or manually:**
   ```bash
   # Create virtual environment
   python3 -m venv venv
   
   # Activate virtual environment
   source venv/bin/activate
   
   # Install dependencies
   pip install -r requirements.txt
   ```

## Running the Application

1. **Activate the virtual environment:**
   - Windows: `venv\Scripts\activate.bat`
   - Linux/macOS: `source venv/bin/activate`

2. **Run the application:**
   ```bash
   python main.py
   ```

3. **Open your browser to:**
   ```
   http://localhost:8000
   ```

## API Endpoints

- `GET /` - Returns the main HTML page with "This is to learn CICD" message
- `GET /health` - Health check endpoint returning application status

## Project Structure

```
├── main.py              # FastAPI application
├── requirements.txt     # Python dependencies
├── setup.bat           # Windows setup script
├── setup.sh            # Linux/macOS setup script
├── README.md           # This file
└── venv/               # Virtual environment (created after setup)
```

## CI/CD Ready

This project is structured to be easily integrated into CI/CD pipelines with:
- Clear dependency management
- Health check endpoint for monitoring
- Simple deployment structure
- Virtual environment isolation

## Dependencies

- **FastAPI**: Modern web framework for building APIs
- **Uvicorn**: ASGI server for running FastAPI applications
