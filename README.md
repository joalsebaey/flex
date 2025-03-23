# FLEX API

FastAPI backend for the FLEX application with MongoDB integration, featuring workout planning and scheduling.

## Features

- OAuth2 JWT-based authentication
- AI-generated workout planning
- MongoDB integration for data persistence
- Dockerized deployment

## Getting Started

### Prerequisites

- Python 3.9+
- MongoDB
- Docker (optional)

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/flex-api.git
   cd flex-api
   ```

2. Create a virtual environment and install dependencies:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Create a `.env` file from the example:
   ```
   cp .env.example .env
   ```
   Edit the `.env` file and add your configuration values.

4. Run the application:
   ```
   uvicorn app.main:app --reload
   ```

### Docker Deployment

1. Build and run with Docker Compose:
   ```
   docker-compose up -d
   ```

## API Documentation

Once the application is running, visit:
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## Testing

Run tests with pytest:
```
pytest
```

## Project Structure

- `app/`: Main application code
  - `controllers/`: Business logic
  - `models/`: Pydantic models
  - `routers/`: API endpoints
  - `config/`: Configuration settings
  - `utils/`: Utility functions
- `tests/`: Test suite
- `docker/`: Docker configuration files

## License

[MIT License](LICENSE)
