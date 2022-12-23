# Building app
FROM node:16.14.2 as build

WORKDIR /app

COPY . .

RUN npm ci --silent
RUN npm run build -- --deploy-url /home/

# Starting NGINX
FROM nginx

COPY ./nginx.conf /etc/nginx/nginx.conf

COPY --from=build /app/dist/home /usr/share/nginx/html