FROM node:8.9.3
COPY . /opt/codepush-server
WORKDIR /opt/codepush-server
RUN npm install
ENV NODE_ENV production
ENV PORT 8080
ENV CONFIG_FILE /opt/codepush-server/config/config.docker.js
ENV DATA_DIR /opt/codepush-server/data
ENV STORAGE_DIR /opt/codepush-server/storage

RDS_USERNAME data_center
RDS_PASSWORD ZdvvtTWQXMf22cv8
DATA_BASE code-push
RDS_HOST rm-bp1s7feggy021u476o.mysql.rds.aliyuncs.com
RDS_PORT 3306

VOLUME [ "/tmp", "/opt/codepush-server/data", "/opt/codepush-server/storage" ]
EXPOSE 8080
CMD [ "./bin/www" ]