# Use an official python image as base
FROM python:3.9

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Set the working directory
WORKDIR /code

# Install dependencies
COPY requirements.txt .
RUN pip install -r requirements.txt

# Copy the rest of the code
COPY . .

# Expose port 8000
EXPOSE 8000

# Start the app
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
