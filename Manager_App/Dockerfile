FROM python:3.9

WORKDIR /app

# Install system dependencies
RUN apt-get update \
    && apt-get install -y build-essential libffi-dev libssl-dev rustc cargo

# Copy requirements.txt to the container
COPY requirements.txt .

# Install Python dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the project code to the container
COPY . .

# Set the entrypoint or CMD according to your application
