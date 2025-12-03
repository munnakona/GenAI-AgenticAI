# Hello MCP Tool

This is my **first MCP tool**, designed to run as a simple example within the **Claude Desktop Environment**. It demonstrates how to create and deploy a basic MCP server with a callable tool.

---

## Features

- Provides a simple **`add(a, b)`** function that returns the sum of two numbers.
- Built using **FastMCPServer**.
- Designed to work with the **Claude Desktop environment** for local testing.
- Serves as a starting point for creating more advanced MCP tools.

---

## Installation

1. Clone this repository:

```bash
git clone https://github.com/munnakona/GenAI-AgenticAI.git
cd GenAI-AgenticAI/hello_mcp

Set up the virtual environment:

uv venv
source .venv/bin/activate


Install dependencies:

uv add mcp-server

Usage

Run the MCP server locally:

uv run hello.py


The server starts and waits for JSON-RPC requests. For example, Claude or any MCP-compatible client can call the add tool.

Tool Example
# Example call to the tool (via client)
result = add(2, 3)
print(result)  # Output: 5

File Structure
hello_mcp/
├── hello.py          # Main MCP server script
├── .venv/            # Virtual environment (ignored in git)
├── README.md         # This file
└── requirements.txt  # (Optional) dependency list

Contributing

Feel free to fork this repository and build your own MCP tools. You can add new functions decorated with @mcp.tool() in hello.py.

License

This project is licensed under the MIT License. See LICENSE for details.

Notes

Ensure the virtual environment is activated before running the server.

Only mcp-server is required for running the FastMCPServer.

This tool is designed for local experimentation and learning purposes.
