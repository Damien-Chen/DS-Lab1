FROM python:latest

# WORKDIR /client
ADD client.py /client/

WORKDIR /client/
# # RUN apt-get update && \
# #     apt-get install -y python3-pip

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY client.py .

CMD ["python", "client.py"]

