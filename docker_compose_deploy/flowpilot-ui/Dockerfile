FROM node:22.18.0-slim AS builder

RUN corepack enable && corepack prepare yarn@4.4.1 --activate

COPY ./frontend /app/flowpilot/
WORKDIR /app/flowpilot
ENV BROWSERSLIST_IGNORE_OLD_DATA=true

RUN yarn install --immutable && yarn build


FROM nginx:1.24.0-alpine
LABEL maintainer=abubakarkhalid637@gmail.com

COPY docker_compose_deploy/flowpilot-ui/nginx.conf /etc/nginx/nginx.conf

COPY --from=builder /app/flowpilot/build/ /usr/share/nginx/html/

RUN mkdir /var/log/flowpilot/
EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
