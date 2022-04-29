FROM python:3.9-alpine

RUN apk add git
RUN apk update
RUN git clone https://github.com/mikhailBrann/test-project-from-docker.git

RUN pip install -r /test-project-from-docker/requirements.txt
EXPOSE 8000

CMD ["python", "/test-project-from-docker/manage.py", "runserver", "0.0.0.0:8000", "--noreload"]


