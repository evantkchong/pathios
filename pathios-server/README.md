# Pathios Server

This API Server is the backend for the Pathios PWA.

Development targets Python 3.11

## Quickstart

1. Install required packages for the server to run via `pip install -r requirements.txt` from this directory.
2. Run the server via `uvicorn core.main:app --reload`. This starts the server and makes it restart whenever code changes are detected.

## Docker
1. Ensure you already have docker installed.
2. Build the docker image for this server using `docker build -t pathios-server .`
3. Run a docker container based on the image we just built using `docker run -p 8080:8080 pathios-server`.
