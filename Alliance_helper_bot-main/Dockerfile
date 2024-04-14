
FROM python:3.12.0

COPY . /app


WORKDIR /app

RUN pip install pipenv


COPY Pipfile Pipfile.lock /app/
RUN pipenv install --deploy --ignore-pipfile Alliance_helper_bot-main

CMD ["pipenv", "run", "python", "Alliance_helper_bot-main/your_personal_assistant_script.py"]

