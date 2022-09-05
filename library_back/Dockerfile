FROM python:3.10.4

ENV PYTHONUNBUFFERED = 1

WORKDIR /code

COPY ./requirements.txt .
RUN pip install -r requirements.txt
COPY entrypoint.sh /usr/bin/
RUN chmod +x /usr/bin/entrypoint.sh

ENTRYPOINT ["entrypoint.sh"]