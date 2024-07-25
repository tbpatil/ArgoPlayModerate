# Use the official Python base image
FROM python:3.11-alpine

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# # Install additional packages for GUI support
# RUN apt-get update && apt-get install -y \
#     && rm -rf /var/lib/apt/lists/*

# Set the environment variable to allow GUI
# ENV DISPLAY=:0

# Expose port 5000 (or the port your app runs on)
EXPOSE 5000

# Run the application
CMD ["python", "app.py"]
