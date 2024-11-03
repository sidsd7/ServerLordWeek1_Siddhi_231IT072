# In flask/Dockerfile

# Use an appropriate base image for Python
FROM python:3.9

# Set the working directory in the container
WORKDIR /app

# Copy the Flask app code into the container
COPY . /app

# Install dependencies
RUN pip install -r requirements.txt

# Expose the port Flask runs on
EXPOSE 5050

# Run the Flask app
CMD ["python", "main.py"]
