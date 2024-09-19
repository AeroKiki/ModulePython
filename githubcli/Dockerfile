# Start with the FastAPI base image
FROM tiangolo/uvicorn-gunicorn-fastapi:python3.9

# Set the working directory
WORKDIR /app

# Copy the application code to the container
COPY . /app

# Install dependencies
RUN pip install --no-cache-dir firebase-admin pydantic

# Expose port 8001
EXPOSE 8001

# Optionally copy .env file and set environment variable (if needed)
# COPY .env /app
ENV ENV_FILE_LOCATION=/app/.env
