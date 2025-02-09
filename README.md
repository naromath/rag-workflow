# RAG Workflow Project

This project implements a Retrieval-Augmented Generation (RAG) workflow using OpenAI Embeddings. It provides a FastAPI application that allows users to query information and receive generated responses based on the retrieved data.

## Project Structure

```
rag-workflow
├── app
│   ├── __init__.py
│   ├── main.py                # Entry point of the FastAPI application
│   ├── api
│   │   ├── __init__.py
│   │   └── endpoints.py       # Defines API endpoints
│   ├── core
│   │   ├── __init__.py
│   │   └── config.py          # Configuration settings
│   ├── models
│   │   ├── __init__.py
│   │   └── embeddings.py       # Data structures and functions for embeddings
│   ├── services
│   │   ├── __init__.py
│   │   └── rag_service.py      # Core logic for RAG workflow
│   └── utils
│       ├── __init__.py
│       └── helpers.py          # Utility functions
├── tests
│   ├── __init__.py
│   └── test_endpoints.py       # Unit tests for API endpoints
├── requirements.txt             # External dependencies
├── .env                          # Environment variables
└── README.md                    # Project documentation
```

## Setup Instructions

1. **Clone the repository:**
   ```
   git clone <repository-url>
   cd rag-workflow
   ```

2. **Create a virtual environment:**
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies:**
   ```
   pip install -r requirements.txt
   ```

4. **Set up environment variables:**
   Create a `.env` file in the root directory and add your OpenAI API key:
   ```
   OPENAI_API_KEY=your_api_key_here
   ```

## Usage

To run the FastAPI application, execute the following command:
```
uvicorn app.main:app --reload
```

You can access the API documentation at `http://127.0.0.1:8000/docs`.

## Testing

To run the tests, use the following command:
```
pytest tests/
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.# rag-workflow
