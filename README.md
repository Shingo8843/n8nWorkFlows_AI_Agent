# n8n Workflows Collection

This repository contains a collection of n8n workflows that leverage AI and automation capabilities. Each workflow is designed to solve specific use cases and can be easily imported into your n8n instance.

## Workflows

### AI Brave Search Agent
- **Location**: `workflows/ai_brave_search_agent/`
- **Description**: An AI-powered search assistant that combines Ollama's Qwen3 model with Brave Search capabilities
- **Key Features**:
  - Natural language query processing
  - Context-aware conversations
  - Intelligent web search execution
  - Memory buffer for conversation history
- **Requirements**:
  - Ollama with Qwen3 model
  - Brave API credentials
  - n8n nodes: @n8n/n8n-nodes-langchain, n8n-nodes-mcp

[View Detailed Documentation](workflows/ai_brave_search_agent/README.md)

## Getting Started

1. Clone this repository
2. Import the desired workflow into your n8n instance
3. Configure the required credentials and environment variables
4. Follow the specific setup instructions in each workflow's README

## Prerequisites

- Running n8n instance
- Required API credentials (varies by workflow)
- Docker (if using docker-compose setup)

## Environment Setup

The repository includes a `docker-compose.yml` file for easy deployment. Required environment variables:

```env
N8N_COMMUNITY_PACKAGES_ALLOW_TOOL_USAGE=true
MCP_BRAVE_API_KEY=your_brave_api_key
FIRECRAW_API_KEY=your_firecraw_api_key
```

## Contributing

Feel free to:
1. Fork the repository
2. Create a new branch for your workflow
3. Add your workflow with proper documentation
4. Submit a pull request

