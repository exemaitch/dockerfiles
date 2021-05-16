
FROM python:3.9-slim-buster

#  Install the pip requirements
COPY requirements.txt /tmp/pip/
RUN pip3 --disable-pip-version-check --no-cache-dir install -r /tmp/pip/requirements.txt \
    && rm -rf /tmp/pip

# RUN pre-commit install
WORKDIR /app

ENTRYPOINT ["jupyter"]