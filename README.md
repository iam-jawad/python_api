# DateTime API

This is a simple FastAPI-based Python project that provides an API endpoint to fetch the current date and time in ISO format.

## Features

- Returns the current date and time in UTC.
- Uses FastAPI for lightweight and high-performance API handling.
- Dockerized for easy deployment.

## Project Structure

```
datetime-api/
│── app.py             # FastAPI application
│── requirements.txt   # Dependencies
│── Dockerfile         # Docker configuration
│── README.md          # Project documentation
```

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Docker

### Running with Docker

1. Clone the repository:
   ```sh
   git clone https://github.com/iam-jawad/python_api.git
   cd datetime-api
   ```
2. Build the Docker image:
   ```sh
   docker build -t datetime-api .
   ```
3. Run the container:
   ```sh
   docker run -p 8000:8000 datetime-api
   ```
4. Access the API at:
   ```
   http://localhost:8000/datetime
   ```

### Example Response

```json
{
  "current_datetime": "2024-02-26T12:34:56.789123"
}
```
