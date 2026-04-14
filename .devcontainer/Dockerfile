FROM mcr.microsoft.com/devcontainers/python:1-3.11-bookworm

RUN apt-get update \
    && apt-get install -y curl ca-certificates git \
    && rm -rf /var/lib/apt/lists/*

RUN curl -LsSf https://astral.sh/uv/install.sh | sh \
    && cp /root/.local/bin/uv /usr/local/bin/uv \
    && cp /root/.local/bin/uvx /usr/local/bin/uvx
