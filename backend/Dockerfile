FROM python:3.8-alpine

WORKDIR /app

ENV FLASK_APP=main.py

ENV FLASK_ENV=development

ENV FLASK_RUN_HOST=0.0.0.0

ENV MONGO_URI="mongodb+srv://udollar:GcVqF7W69mM88v9u@cluster0.sqhdi.mongodb.net/erate?retryWrites=true&w=majority"

RUN apk add --no-cache gcc musl-dev linux-headers

COPY requirements.txt requirements.txt

RUN pip install -r requirements.txt

EXPOSE 8000

COPY . .

CMD ["flask", "run"]

