FROM maven:3-jdk-8
ENV DB_HOST_IP="localhost"
WORKDIR /usr/src/app # container預設路徑
COPY . ./
COPY wait-for-it.sh ./wait-for-it.sh
RUN chmod +x wait-for-it.sh # 設定執行指定檔案 像 windows執行 exe檔一樣
RUN mvn clean package # java使用
CMD java -jar target/accessing-data-mysql-0.0.1-SNAPSHOT.jar # 專案建立起來以後的初始指令

