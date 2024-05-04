FROM python:3-slim
WORKDIR /programas/api-students
RUN apt-get update && apt-get install -y curl && pip3 install flask
COPY . .
RUN python3 db.py
CMD [ "python3", "./app.py" ]
