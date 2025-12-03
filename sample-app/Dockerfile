# Use official Python slim image
FROM python:3.12-slim

WORKDIR /app

# Install dependencies
COPY requirements.txt .
RUN python -m pip install --no-cache-dir -r requirements.txt

# Copy app
COPY . .

# Expose port and run
ENV PORT=5000
EXPOSE 5000

# Use a simple command to run the app
CMD ["python", "app.py"]
