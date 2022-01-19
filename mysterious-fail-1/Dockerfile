FROM python:3.8-slim
USER jenkins
COPY requirements.txt /app/
WORKDIR /app
RUN pip install -r requirements.txt
RUN useradd -ms /bin/bash jenkins -u 113 -g 120
COPY . /app

CMD ["python3", "reverse_figlet.py"]
