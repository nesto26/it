# Use an official Ubuntu as a base image
FROM ubuntu:20.04

# Set environment variables to disable interactive prompts
ENV DEBIAN_FRONTEND=noninteractive

# Update package list and install dependencies
RUN apt-get update && apt-get install -y --no-install-recommends \
    wget \
    curl \
    vim \
    unzip \
    git \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory inside the container
WORKDIR /app

# Copy your application code into the container
COPY . /app

# Define the entry point for the container (optional)
CMD ["bash"]
