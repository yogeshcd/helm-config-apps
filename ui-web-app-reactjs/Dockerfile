#docker build -t val418orant/ui-reactjs:latest .
#docker push val418orant/ui-reactjs:latest

FROM node:8
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build 
EXPOSE 8080
CMD ["node", "server.js"]