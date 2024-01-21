FROM python:3.11.2

RUN pip install --upgrade pip

COPY ./django/requirements.txt .
RUN pip install -r requirements.txt

COPY ./django /app

WORKDIR /app

COPY ./entrypoint.sh /
ENTRYPOINT ["sh", "/entrypoint.sh"]