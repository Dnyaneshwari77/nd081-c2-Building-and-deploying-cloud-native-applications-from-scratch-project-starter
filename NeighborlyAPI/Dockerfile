# Use official Azure Functions Python base image
FROM mcr.microsoft.com/azure-functions/python:4-python3.8


# Set working directory
WORKDIR /home/site/wwwroot

# Copy function app files
COPY . /home/site/wwwroot

# Install dependencies
RUN pip install --upgrade pip setuptools wheel --timeout 120
RUN pip install -r requirements.txt --timeout 120
# Expose port (optional, default for Azure Functions)
EXPOSE 80

