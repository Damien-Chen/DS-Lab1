FROM python:latest

WORKDIR /server

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY server.py .

# set environment variables
ENV FLASK_APP=server.py
ENV FLASK_RUN_HOST=0.0.0.0
ENV debug=True

CMD ["python", "server.py", "--host=0.0.0.0"]

EXPOSE 5000
