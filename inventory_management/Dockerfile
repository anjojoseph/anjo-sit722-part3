# Dockerfile for inventory_management microservice
FROM python:3.11-alpine

WORKDIR /app/

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

#COPY app ./

COPY . .

#COPY ./app /app

#COPY ./main.py /apkub


CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8001"]
