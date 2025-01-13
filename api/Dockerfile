FROM python:3.11

WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir --upgrade -r /code/requirements.txt
COPY . .

EXPOSE 8080

CMD ["unicorn", "run", "app/main.py", "--port", "80"]