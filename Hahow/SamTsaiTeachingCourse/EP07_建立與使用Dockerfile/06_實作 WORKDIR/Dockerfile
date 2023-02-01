FROM alpine:latest

ENV myworkdir /var/www/localhost/htdocs/ #設定共用變數

WORKDIR ${myworkdir} #設定初始目錄位置

RUN apk --update add apache2
RUN rm -rf /var/cache/apk/*

RUN echo "<h3>I am Sam. Iam taking this great Docker Course. Round 01<h3>" >> index.html
RUN echo "<h3>I am Sam. Iam taking this great Docker Course. Round 02<h3>" >> index.html
RUN echo "<h3>I am Sam. Iam taking this great Docker Course. Round 03<h3>" >> index.html

MAINTAINER MyName

ENTRYPOINT ["httpd", "-D", "FOREGROUND"] #預設啟動指令