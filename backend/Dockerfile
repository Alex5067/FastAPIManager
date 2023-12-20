FROM python:bullseye

# Установка рабочей директории внутри контейнера
WORKDIR /app
# Копирование зависимостей проекта и установка их через pip
COPY requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt
RUN pip install uvicorn
# Копирование всего содержимого папки backend внутрь контейнера
COPY . /app
#EXPOSE 8000

# Команда для запуска FastAPI
#CMD ["uvicorn", "main:app", "--host", "127.0.0.1", "--port", "8000"]
