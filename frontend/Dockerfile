FROM node:14.16.1
WORKDIR /app
COPY backend/package.json .
COPY backend/package-lock.json .
RUN npm install
COPY frontend/. .
COPY backend/common/. ./server/common/
RUN npm install
ENTRYPOINT npm run start