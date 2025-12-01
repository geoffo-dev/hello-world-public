FROM python:3.13-slim

WORKDIR /app

# Install dependencies
RUN pip install --no-cache-dir flask

# Copy app
COPY main.py .

EXPOSE 8000

CMD ["python", "main.py"]
