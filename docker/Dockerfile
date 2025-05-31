# docker/Dockerfile

FROM python:3.11-slim
WORKDIR /app

COPY ./quant_trading /app/quant_trading
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

CMD ["uvicorn", "quant_trading.api:app", "--host", "0.0.0.0", "--port", "8000"]
