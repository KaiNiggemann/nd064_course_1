FROM python:3.8
LABEL maintainer="Kai Niggemann"

COPY ./techtrends /app
WORKDIR /app
RUN pip install -r requirements.txt

EXPOSE 3111

# command to run on container start
CMD [ "python", "init_db.py" ]
CMD [ "python", "app.py" ]
