# Use official Python image
FROM python
# Set working directory
WORKDIR /app
# Copy requirement file and install dependencies
COPY requirements.txt .
RUN pip install -r requirements.txt
# Copy application code
COPY . .
# Expose port 5000
EXPOSE 5000
# Run the app
CMD ["python", "app.py"]
