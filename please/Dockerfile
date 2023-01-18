FROM node:16.15.1-alpine AS build-env
ENV NODE_ENV=production
WORKDIR /app
COPY ./package*.json ./
RUN npm install
RUN npm install esm
RUN ls
COPY ./ ./
ENV PORT=80
EXPOSE 80
CMD [ "npm", "start" ]