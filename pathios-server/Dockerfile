FROM python:3.11-slim-bullseye

WORKDIR /pathios
COPY ./requirements.txt /pathios/requirements.txt
RUN pip install --no-cache-dir --upgrade -r /pathios/requirements.txt
COPY ./core /pathios/core

CMD ["uvicorn", "core.main:app", "--host", "0.0.0.0", "--port", "8080"]
