FROM python:3.9.17-slim-buster

RUN apt update -y && apt install awscli -y

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . /app

CMD ["python3", "app.py"]