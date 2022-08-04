FROM python:3.8

WORKDIR /app

RUN pip install --upgrade pip 
COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .

EXPOSE 8000

#ENTRYPOINT ["python manage.py migrate"]

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]