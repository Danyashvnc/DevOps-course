FROM python:3.13-slim-bookworm

LABEL course.student="Danyashvnc"

WORKDIR /app
ENV PYTHONUNBUFFERED=1 PYTHONDONTWRITEBYTECODE=1

COPY app.py index.html ./

RUN mkdir -p /data && chown 10001:10001 /data
USER 10001:10001

EXPOSE 8000
CMD ["python", "app.py"]
