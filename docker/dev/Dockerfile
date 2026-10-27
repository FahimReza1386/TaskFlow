
FROM python:3.13-slim

ENV PYTHONUNBUFFERED=1
ENV PYTHONDONTWRITEBYTECODE=1

WORKDIR /usr/src/app

COPY requirements.txt .

RUN pip install --no-cache-dir -i https://package-mirror.liara.ir/repository/pypi/simple -r requirements.txt

COPY core/ .

CMD ["python", "manage.py", "runserver", "0.0.0.0:8088"]
