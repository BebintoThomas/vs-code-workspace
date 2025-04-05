# filepath: c:\Users\benix\OneDrive\Desktop\vs code workspace\dockerfile
# Use an official Python runtime
FROM python:3.9

WORKDIR /app

# Copy the app directory into the container
COPY ./app /app

RUN pip install flask

# Set FLASK_APP explicitly
ENV FLASK_APP=app.py
ENV FLASK_RUN_HOST=0.0.0.0
ENV FLASK_RUN_PORT=5000

EXPOSE 5000

CMD ["python", "app.py"]