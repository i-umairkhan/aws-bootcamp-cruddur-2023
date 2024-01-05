FROM python:3.10-slim-buster

# Setting Work Dir to /backend-flask
WORKDIR /backend-flask

COPY requirements.txt requirements.txt

# Installing required packages
RUN pip install -r requirements.txt

COPY . .

# Setting ENV Vars
ENV FLASK_ENV=development
ENV FRONTEND_URL="*"
ENV BACKEND_URL="*"

EXPOSE ${PORT}

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]




