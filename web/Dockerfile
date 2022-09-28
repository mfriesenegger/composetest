FROM registry.suse.com/bci/python:latest@sha256:a9d9d549d0da66d90b9c2e70298747260013869660edec3a7f117b0e47779f8a
WORKDIR /code
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0
RUN pip install redis flask
RUN curl -sL -o app.py https://raw.githubusercontent.com/mfriesenegger/composetest/main/web/app.py
CMD ["flask", "run"]
