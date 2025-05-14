# AI Brave Search Agent Workflow

This n8n workflow implements an AI agent that can perform web searches using Brave Search capabilities. The workflow combines the power of Ollama's language model with Brave's search functionality to create an intelligent search assistant.

## Components

1. **AI Agent**: The main agent node that coordinates the workflow and processes user input
2. **Ollama Chat Model**: Uses the Qwen3 model for natural language processing
3. **Simple Memory**: Maintains conversation context using a buffer window
4. **Brave Actions**: Provides access to Brave's search capabilities
5. **Brave Search Execute**: Executes specific search tools based on the AI agent's decisions

## Prerequisites

- n8n instance running
- Ollama installed and configured with Qwen3 model
- Brave API credentials configured in n8n
- Required n8n nodes:
  - @n8n/n8n-nodes-langchain
  - n8n-nodes-mcp

## Setup

1. Import the workflow.json file into your n8n instance
2. Configure the following credentials:
   - Ollama API credentials
   - Brave API credentials
3. Ensure the Qwen3 model is available in your Ollama installation

## Usage

The workflow can be triggered with natural language queries. The AI agent will:
1. Process the input using the Qwen3 model
2. Determine if a search is needed
3. Execute appropriate Brave search actions
4. Return relevant results

## Environment Variables

The following environment variables are required:
- MCP_BRAVE_API_KEY: Your Brave API key

## Notes

- The workflow uses a memory buffer to maintain context between interactions
- The system message can be customized in the AI Agent node to change the assistant's behavior
- The workflow is designed to be extensible for additional search capabilities 