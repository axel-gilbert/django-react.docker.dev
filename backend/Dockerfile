# Use a base image of Python 3 on Alpine Linux
FROM python:3-alpine

# Set the environment variable PYTHONUNBUFFERED to 1.
# This ensures that Python output is logged immediately, which is useful when debugging.
ENV PYTHONUNBUFFERED 1

# Create a working directory inside the container named /code
RUN mkdir /code

# Set the working directory to /code. All subsequent commands will be run from this directory.
WORKDIR /code

# Copy requirements.txt into the container at location /code/
# This file contains a list of Python packages required by the application.
COPY requirements.txt /code/

# Run pip (Python's package installer) to install the dependencies specified in requirements.txt
RUN pip install -r requirements.txt

# Copy the rest of the application's code into the container at location /code/
COPY . /code/
