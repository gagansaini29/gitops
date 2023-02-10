FROM python:3.10.0-alpine3.15
WORKDIR /app
RUN apt-get update
 RUN apt-get install -y swig
 RUN apt-get install -y python-dev
 RUN apt-get install -y libssl-dev
COPY . /app
# COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY . /app
EXPOSE 8000
CMD ["python","manage.py","runserver","0.0.0.0:8000"]