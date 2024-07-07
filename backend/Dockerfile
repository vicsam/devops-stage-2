
FROM python:3.8-slim


WORKDIR /app


RUN pip install --no-cache-dir uvicorn==0.15.0 fastapi==0.68.2


COPY . .


RUN chmod +x /usr/local/bin/uvicorn


EXPOSE 8000


CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
