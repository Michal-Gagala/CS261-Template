# syntax=docker/dockerfile:1
FROM python:3.8-bullseye

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1


WORKDIR /src
COPY requirements.txt /src/
RUN pip install -r requirements.txt

EXPOSE 8000

COPY . /src/

# ENTRYPOINT ["ls"]
# ENTRYPOINT ["python3", "backend/manage.py"]
# CMD ["makemigrations", "migrate", "runserver", "0.0.0.0:8000"]

CMD ["backend/start.sh"]
# CMD ["ls"]
