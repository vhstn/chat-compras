FROM rasa/rasa-sdk:3.6.2

WORKDIR /app

COPY requirements-actions.txt ./

USER root

RUN pip install --no-cache-dir -r requirements-actions.txt

USER ${USER_ID:-1001}

COPY . .