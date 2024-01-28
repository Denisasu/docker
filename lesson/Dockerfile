FROM python:3.12-alpine

WORKDIR .

COPY requirements.txt .
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

COPY . .

CMD [ "uvicorn", "app:app", "--host", "0.0.0.0", "--port", "6090"] 