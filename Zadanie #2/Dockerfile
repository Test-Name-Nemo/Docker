FROM python:3.12

WORKDIR /web-app

COPY ./web-app /web-app

RUN pip install -r /web-app/requirements.txt

ENV SECRET_KEY 
ENV DEBUG

RUN python manage.py migrate

CMD ["gunicorn", "--bind", "0.0.0.0:8000", "webpython.wsgi"]