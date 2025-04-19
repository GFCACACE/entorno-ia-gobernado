FROM python:3.11-slim
COPY . /app
WORKDIR /app
RUN pip install mcpo uv
# Replace with your MCP server command; example: uvx mcp-server-time
CMD ["uvx", "mcpo", "--port", "8000", "--api-key", "top-secret", "--", "mcpo", "--config", "./config.json"]