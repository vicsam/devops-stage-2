
FROM python:3.8-slim


WORKDIR /app


RUN pip install uvicorn


COPY . .


RUN chmod +x /usr/local/bin/uvicorn


EXPOSE 8000


CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
