# Use Python for Django
FROM python:latest

# Set the working directory
WORKDIR /app

# Copy requirements and install dependencies
COPY requirements2.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy the Django project files
COPY . .

# Expose port 8001 for Django
EXPOSE 8001

# Start the Django development server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8001"]