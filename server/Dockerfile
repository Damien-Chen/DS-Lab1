FROM python:latest

WORKDIR /

COPY requirements.txt .


RUN pip install -r requirements.txt && mkdir data

COPY server.py .

# set environment variables
ENV FLASK_APP=server.py
ENV FLASK_RUN_HOST=0.0.0.0

EXPOSE 5000

COPY . .
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0", "--port=5000"], 
# CMD ["python", "server.py", "run", "--host=0.0.0.0"]

