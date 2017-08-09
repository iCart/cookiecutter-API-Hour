FROM python:3

ENV PROJECT={{cookiecutter.app_name}}

# Copy teh code
COPY . /opt/$PROJECT

RUN pip install -r /opt/$PROJECT/requirements.txt
WORKDIR /opt/$PROJECT
CMD api_hour -ac $PROJECT:Container

