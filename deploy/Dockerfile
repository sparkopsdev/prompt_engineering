FROM python:3.14-trixie

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1
ENV PIP_NO_CACHE_DIR=1

RUN apt-get update && apt-get install -y \
    build-essential \
    git \
    curl \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace

COPY requirements.txt requirements.txt

RUN pip install --upgrade pip && \
    pip install jupyterlab ipython && \
    pip install -r requirements.txt

EXPOSE 8888