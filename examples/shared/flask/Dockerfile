FROM python:3.10.6-slim-bullseye@sha256:2a1ffc203358817ab0be746142ad3667954b752dfe62e8df385536e5a1e1dcbd

ADD requirements.txt /tmp/flask-requirements.txt
RUN pip3 install -qr /tmp/flask-requirements.txt
RUN mkdir /code

ENTRYPOINT ["python3", "/code/service.py"]
