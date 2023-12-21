FROM python:bullseye

RUN apt-get update && apt-get install -y git
ARG GIT_BRANCH=main
RUN git clone -b ${GIT_BRANCH} https://github.com/Alex5067/FastAPIManager.git /app

WORKDIR /app/backend
RUN git checkout ${GIT_BRANCH}

RUN pip install -r requirements.txt
RUN pip install uvicorn
