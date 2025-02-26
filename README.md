# Hands-on Implementation of Agentic Systems using LlamaIndex

This repository contains a Jupyter Notebook that provides a hands-on implementation of **Agentic Systems** using LlamaIndex workflows. Here, we have created a **ReAct Agent** that has access to three tools:
- **Two Query Engine Tools**
- **One Web Search Tool**

All of this is implemented using the **event-driven LlamaIndex workflows**.

## Overview
ReAct agents are agents that can **reason** and then **take action**. To loop over their decisions and make the next best decision, the **LlamaIndex event-driven architecture** enables efficient implementation of this behavior.

## Installation
Before running the notebook, install the required dependencies:
```bash
pip install llama-index==0.12.17
pip install faiss-cpu==1.10.0
pip install llama-index-vector-stores-faiss==0.3.0
pip install llama-index-embeddings-azure-openai==0.3.0
pip install llama-index-llms-azure-openai==0.3.0
pip install llama-index-utils-workflow==0.2.1
pip install duckduckgo-search==7.3.2
pip install python-dotenv==1.0.1
```

## Environment Setup
Ensure that your API keys and environment variables are properly set up by using a `.env` file:
```python
from dotenv import load_dotenv
import os

# Load environment variables from .env file
load_dotenv()
```

## Running the Notebook
1. Open the Jupyter Notebook in VS Code or Jupyter Lab:
   ```bash
   jupyter notebook Webinar_Demo_LLamaIndex_Workflows.ipynb
   ```
2. Follow the step-by-step workflow to set up the agent.

## Key Features
- **Asynchronous Execution**: Enables efficient task execution without blocking operations.
- **Event-Driven Architecture**: Facilitates real-time decision-making and looping over actions.
- **Dynamic Tool Selection**: The ReAct agent chooses the best tool based on the query.
- **Memory and Reflection**: The agent can reflect on past interactions and adjust its responses.

