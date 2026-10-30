FROM mcr.microsoft.com/devcontainers/python:3-3.12
# Links the GHCR package to this repo.
LABEL org.opencontainers.image.source=https://github.com/riverside-pirates/computer-science-essentials
# Baked in so `python -m pytest` works the moment the codespace opens.
RUN pip install --no-cache-dir pytest
