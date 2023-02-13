FROM python:3.10.0-alpine3.15
WORKDIR /app
COPY . /app
# COPY requirements.txt requirements.txt
CMD [ "ls" ]
RUN pip install -r requirements.txt
COPY . /app
EXPOSE 8000

# CMD ["python","manage.py","runserver","0.0.0.0:8000"]