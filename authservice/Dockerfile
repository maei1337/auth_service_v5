FROM python:3
LABEL maintainer "Private Capital Hub"
WORKDIR /usr/src/app
ENV FLASK_APP=app.py
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt && pip install gunicorn
COPY . .
EXPOSE 8000
CMD /usr/src/app/boot.sh
