# README

更新時間: 2021-04-01

**專案目標:**

- 在 ubuntu 上面安裝 docker, docker-compose
- 下載 mysql 8.0 的 image，並起一個 container
- 資料庫管理工具: phpMyadmin

---

## 步驟

1. git clone repo   ---> 下載這個 repo
2. cd docker_mysql  ---> 進入 repo
3. cp env_example .env  ---> 將範本複製一份，並且取名為.env。這樣做是因為不要讓Github上面看到密碼。
4. vim .env  ---> 更改 .env 的參數。

    應該需要更改兩個地方

    - MYSQL_PASSWORD=xxx  ---> xxx改成自己的 password
    - MYSQL_Volumn_local=xxx  ---> xxx改成 /datamount/vol/mysql

5. 在 docker_mysql/ 資料夾下，下指令 `docker-compose up -d`

啟動成功(開心~ 灑花~)

--

port 的部分在 docker-compose.yml 檔案裡面有

- 3306: mysql
- 8080: phpmyadmin

---

## 技術細節說明

![image01](/image/image01.PNG)

--
![image02](/image/image02.PNG)

--
![image03](/image/image03.PNG)

--
![image04](/image/image04.PNG)

--
![image05](/image/image05.PNG)

---

## END
