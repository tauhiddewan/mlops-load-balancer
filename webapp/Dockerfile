FROM python:3.10-alpine

WORKDIR /webapp

COPY . .

RUN pip install -r requirements.txt

CMD gunicorn --bind 0.0.0.0:5000 wsgi:app