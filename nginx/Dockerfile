FROM nginx:1.17-alpine

# 设置时区
RUN echo "Asia/shanghai" > /etc/timezone;
RUN rm -rf /etc/localtime;
RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

