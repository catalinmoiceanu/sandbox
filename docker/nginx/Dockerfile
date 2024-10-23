FROM nginx:1.27-alpine3.20

ARG APP_ID

RUN echo ${APP_ID}
COPY app.conf /etc/nginx/conf.d/default.conf
RUN sed -i "s/APP_ID/${APP_ID}/g" /etc/nginx/conf.d/default.conf
