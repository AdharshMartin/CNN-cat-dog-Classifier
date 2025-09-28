# Using an official TensorFlow GPU image base
# This image comes pre-installed with TensorFlow, Python, CUDA, and cuDNN
FROM tensorflow/tensorflow:2.16.1-gpu-jupyter

# Install any additional utilities (optional, but good for development)
RUN apt-get update && apt-get install -y \
    git \
    curl \
    vim \
    && rm -rf /var/lib/apt/lists/*

# Set a non-root user (good practice, but TensorFlow images often handle this)
# The default user in this base image is often 'jovyan' (ID 1000).
# The devcontainer setup will automatically handle user configuration.

# Set the working directory (will be overridden by devcontainer.json)
WORKDIR /workspaces/cnn-project
