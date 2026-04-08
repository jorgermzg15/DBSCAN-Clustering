FROM mcr.microsoft.com/devcontainers/python:3.11-bullseye

# Remove yarn repo with expired GPG key to prevent apt-get update failures
RUN rm -f /etc/apt/sources.list.d/yarn.list || true

WORKDIR /workspace

CMD ["sleep", "infinity"]
