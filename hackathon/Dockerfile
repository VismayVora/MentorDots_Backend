FROM python:3.9-slim

ENV PYTHONUNBUFFERED=1

WORKDIR /app

RUN apt-get update

COPY requirements.txt /app/

RUN pip install -r requirements.txt

COPY . /app/


EXPOSE 8080

CMD [ "python", "manage.py", "runserver", "0.0.0.0:8080" ]