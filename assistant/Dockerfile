FROM rasa/rasa_sdk:2.2.0

USER root

COPY actions /app
COPY requirements.txt /app
COPY workshop_data.csv /app

RUN pip3 install -r requirements.txt
CMD["start", "actions", "--actions", "--debug"]

USER 1001