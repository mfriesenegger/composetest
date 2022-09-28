FROM registry.suse.com/bci/python:latest
WORKDIR /code
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0
RUN pip install redis flask
RUN curl -sL -o app.py https://raw.githubusercontent.com/mfriesenegger/composetest/main/web/app.py
CMD ["flask", "run"]
