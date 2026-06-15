FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .
COPY vulnerable-flask-app-linux.py .
COPY test.db .

RUN pip install --no-cache-dir flask werkzeug

EXPOSE 8081

CMD ["python", "vulnerable-flask-app-linux.py"]