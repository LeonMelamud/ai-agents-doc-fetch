# AI Agents Project

## Overview

The AI Agents project is a powerful system that combines file management, vector databases, and large language models (LLMs) to provide intelligent document analysis and question-answering capabilities. It consists of a Python backend built with FastAPI and a JavaScript frontend for user interaction.

## Features

- File upload and management
- Automatic file embedding into a vector database
- Intelligent question-answering about uploaded documents
- Configurable vector database and LLM integrations
- User-friendly web interface

## Prerequisites

- Python 3.8+
- Node.js 14+
- Qdrant vector database (or alternative)
- Access to an LLM API (e.g., OpenAI)

## Setup

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/ai-agents.git
   cd ai-agents
   ```

2. Set up the Python environment:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```

3. Configure the application:
   - Copy `config.yaml.example` to `config.yaml`
   - Edit `config.yaml` to set up your vector database and LLM API credentials

4. Set up the frontend:
   ```
   cd frontend
   npm install
   ```

## Running the Application

1. Start the backend server:
   ```
   uvicorn app.main:app --reload
   ```

2. In a separate terminal, start the frontend development server:
   ```
   cd frontend
   npm run dev
   ```

3. Open your browser and navigate to `http://localhost:3000` (or the port specified by your frontend setup).

## Usage

1. Use the web interface to upload documents.
2. View the list of uploaded documents.
3. Ask questions about the uploaded documents using the query interface.
4. Receive intelligent responses based on the document content.

## API Endpoints

- `POST /upload`: Upload a file
- `GET /files`: Retrieve list of uploaded files
- `POST /query`: Submit a question about uploaded files
- `GET /config`: Retrieve current configuration
- `POST /config`: Update configuration

## Configuration

Edit `config.yaml` to customize:
- Vector database settings
- LLM provider and model settings
- Embedding model settings
- Other application parameters

## Future Enhancements

1. Multi-modal support: Extend the system to handle images, audio, and video files.
2. Advanced querying: Implement more sophisticated querying techniques, such as multi-hop reasoning or chain-of-thought prompting.
3. User authentication: Add user accounts and personalized document collections.
4. Collaborative features: Allow users to share document collections and collaborate on analysis.
5. Automated summarization: Generate summaries of uploaded documents or collections.
6. Data visualization: Implement visualizations of document relationships and query results.
7. API rate limiting and caching: Optimize API usage and improve response times.
8. Document version control: Track changes in documents over time.
9. Integration with external tools: Connect with popular productivity and analysis tools.
10. Mobile app: Develop a mobile application for on-the-go access.
11. Customizable UI: Allow users to personalize the interface and create custom dashboards.
12. Scheduled queries: Implement a feature for running periodic queries and generating reports.
13. Export functionality: Allow users to export query results and analysis in various formats.
14. Fine-tuning capabilities: Provide options for users to fine-tune the LLM on their specific document sets.
15. Multilingual support: Extend the system to work with documents and queries in multiple languages.

## Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for more information.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

If you encounter any issues or have questions, please file an issue on the GitHub repository or contact our support team at support@aiagents.com.