# Base image
FROM python:3.12.10-slim

# Set working directory
WORKDIR /app

# Copy all project files (preserving structure)
COPY . .

# Install dependencies
RUN pip install --upgrade pip && \
    pip install -r requirements.txt

# Expose port (adjust if using a different port)
EXPOSE 5000

# Set environment variables (optional, adjust as needed)
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

# Default command (adjust for your app)
# Example for Flask:
CMD ["python", "matches.py"]