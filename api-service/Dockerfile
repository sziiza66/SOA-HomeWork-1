FROM python:3.11-slim

WORKDIR /service

COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .

CMD ["uvicorn", "service.main:service", "--host", "0.0.0.0", "--port", "8000"]