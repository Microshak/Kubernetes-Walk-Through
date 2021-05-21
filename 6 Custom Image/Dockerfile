FROM python:3.8-slim-buster

COPY . /app
WORKDIR /app
RUN pip install Flask
ENV FLASK_APP=app.py
ENV FLASK_ENV=development
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]