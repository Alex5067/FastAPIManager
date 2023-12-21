FROM node:latest

RUN apt-get update && apt-get install -y git
ARG GIT_BRANCH=main
RUN git clone -b ${GIT_BRANCH} https://github.com/Alex5067/FastAPIManager.git /app

WORKDIR /app/frontend
RUN git checkout ${GIT_BRANCH}

#COPY . /app
RUN npm install
RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]
