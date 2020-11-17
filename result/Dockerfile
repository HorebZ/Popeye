FROM node:12-alpine
WORKDIR /app
COPY . /app
RUN npm install
EXPOSE 80
ENV PORT 80
CMD ["node", "server.js"]