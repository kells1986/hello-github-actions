FROM python:3.6.13-buster

RUN pip install numpy

COPY src/ /src

ENV PYTHONPATH "${PYTHONPATH}:/src"

ADD test.sh /test.sh
RUN chmod +x /test.sh
ENTRYPOINT ["/test.sh"]