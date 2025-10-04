FROM python:3.14.0rc3

WORKDIR /app

COPY requirements.txt /app/

RUN pip install --no-cache-dir -r requirements.txt

COPY . /app/

ENV PYTHONUNBUFFERED=1

CMD ["sh", "-c", "uvicorn main:app --host=0.0.0.0 --port=7150"]