FROM python:3.9-slim

WORKDIR /app

COPY Pipfile Pipfile.lock ./

RUN pip install pipenv && pipenv install --system

COPY . .

EXPOSE 5000

CMD ["python", "app/main.py"]
