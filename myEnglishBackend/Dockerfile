FROM python:3.6-alpine
ENV PYTHONUNBUFFERED 1

RUN mkdir /backend
WORKDIR /backend
ADD ./requirements.txt /backend/requirements.txt
ADD ./requirements_dev.txt /backend/requirements_dev.txt
RUN pip install -r requirements.txt
RUN pip install -r requirements_dev.txt
ADD . /backend

RUN chmod -R a+w /backend && chmod -R 777 /backend


