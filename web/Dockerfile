FROM python:3.10.9-slim

COPY . /app
WORKDIR /app

RUN python3 -m venv /opt/venv && \
    /opt/venv/bin/pip install --upgrade pip && /opt/venv/bin/pip install -r requirements.txt && \
    chmod +x entrypoint.sh

CMD ["/app/entrypoint.sh"]
