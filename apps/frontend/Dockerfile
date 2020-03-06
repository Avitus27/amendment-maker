FROM python:3.7.6
# move to alpine after dev

WORKDIR /src
ENV FLASK_APP app.py
ENV FLASK_RUN_HOST 0.0.0.0
RUN apt install gcc -yq
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY . .
CMD ["flask", "run"]

