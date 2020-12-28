FROM alpine:latest

RUN apk add --update nodejs npm hugo git

EXPOSE 1313
# for now need to be in  yugabyte-db/ running with $(pwd):/app
WORKDIR /app/docs

RUN npm ci
CMD ["npm", "start"]
