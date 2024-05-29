# ImageIQ

ImageIQ is a FastAPI-based application designed to leverage machine learning for analyzing and generating predictions from text and image inputs. It is optimized for scalability and efficiency, making it ideal for real-time data processing applications.

## Key Features

- **FastAPI Framework**: Leverages the high performance and scalability of FastAPI.
- **Machine Learning Integration**: Utilizes advanced machine learning models for comprehensive analysis of text and images.
- **Docker Support**: Fully containerized using Docker to simplify deployment and ensure consistency across different environments.

## Technologies Used

- **FastAPI**: A modern, fast web framework for building APIs with Python 3.7+ based on standard Python type hints.
- **Python**: The primary programming language used.
- **Docker**: Used for containerizing the application to ensure easy deployment and consistent runtime environments across different systems.
- **Uvicorn**: An ASGI server for Python, used to run the FastAPI application.
- **Pillow (PIL)**: Python Imaging Library, used for image processing tasks.
- **Machine Learning Libraries**: Integration of machine learning libraries such as PyTorch or TensorFlow (specific libraries should be detailed in project dependencies).

## Getting Started

Follow these instructions to set up the project locally for development and testing purposes.

### Prerequisites

Ensure you have the following installed:
- Python 3.8 or higher
- Docker (optional, for containerization)

### Installation

Execute the following steps to get your development environment up and running:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/PrinceTp/ImageIQ
   ```
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the application:**
   ```bash
   uvicorn main:app --reload
   ```

### Docker Usage

For running the application within a Docker container, perform the following:

1. **Build the Docker image:**
   ```bash
   docker build -t ml_api .
   ```
2. **Run the Docker container:**
   ```bash
   docker run -p 8000:8000 ml_api
   ```

## API Endpoints

- `GET /`: Returns a simple "Hello World" message.
- `POST /ask`: Accepts `text` and an `image` file, returns processed results.

## Contributing

Contributions to ImageIQ are welcome! Please refer to the contributing guidelines for more details on how to submit pull requests, report issues, or make feature suggestions.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
