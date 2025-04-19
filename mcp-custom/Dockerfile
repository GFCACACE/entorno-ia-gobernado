FROM python:3.11-slim

# Instalar Node.js y npm
RUN apt-get update && \
    apt-get install -y curl && \
    curl -fsSL https://deb.nodesource.com/setup_18.x | bash - && \
    apt-get install -y nodejs && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

COPY . /app
WORKDIR /app
RUN pip install mcpo uv
# Replace with your MCP server command; example: uvx mcp-server-time
CMD ["uvx", "mcpo", "--port", "8000", "--api-key", "top-secret", "--", "mcpo", "--config", "./config.json"]