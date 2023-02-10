# image build phase
FROM node:16
WORKDIR /myapp # 預設目錄
COPY package.json .
RUN npm install # 建置環境
COPY . .
COPY wait-for-it.sh ./wait-for-it.sh
RUN chmod +x wait-for-it.sh # 設定執行指定檔案 像 windows執行 exe檔一樣
# container running phase
CMD ["npm", "start"] # 專案建立起來以後的初始指令


