FROM python:3.8-slim

COPY requirements.txt /app/
WORKDIR /app
RUN pip install -r requirements.txt
RUN addgroup -g 120 jenkins
RUN useradd -ms /bin/bash jenkins -u 113 -g 120
USER jenkins
COPY . /app

CMD ["python3", "reverse_figlet.py"]
