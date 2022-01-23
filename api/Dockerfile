FROM python:3.8

WORKDIR /usr/src/app

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

EXPOSE 8000
COPY . .
RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

RUN apt-get upgrade -y
RUN apt-get update -y

CMD  bash -c "python manage.py runserver 0.0.0.0:8000"
