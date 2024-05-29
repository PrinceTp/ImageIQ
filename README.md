# ImageIQ

This project is a FastAPI application designed to serve a machine learning model that processes text and image inputs to generate predictions. It's built to be scalable and efficient, suitable for real-time data processing.

## Features

- **FastAPI**: Utilizes FastAPI for high performance and easy scalability.
- **Machine Learning Model**: Integrates a machine learning model to analyze text and images.
- **Docker Support**: Containerized with Docker for easy deployment and consistent runtime environments.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

What things you need to install the software and how to install them:

- Python 3.8+
- Docker (optional for containerization)

### Installing

A step by step series of examples that tell you how to get a development environment running:

1. Clone the repository: git clone https://github.com/PrinceTp/ImageIQ
2. Install the required packages: pip install -r requirements.txt 
3. Run the application: uvicorn main:app --reload

### Using Docker

To run the application in a Docker container, follow these steps:

1. Build the Docker image: docker build -t ml_api .
2. Run the Docker container: docker run -p 8000:8000 ml_api


## API Endpoints

- `GET /`: Returns a simple "Hello World" message.
- `POST /ask`: Accepts `text` and an `image` file, returns processed results.
