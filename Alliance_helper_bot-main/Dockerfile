
FROM python:3.12.0


COPY . /app


WORKDIR /app


RUN pip install pipenv


COPY Pipfile Pipfile.lock /app/
RUN pipenv install --deploy --ignore-pipfile

CMD ["pipenv", "run", "python", "setup.py"]
