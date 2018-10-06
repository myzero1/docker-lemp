docker-lemp
========================
This is a lenmp evn builded by docker-compose.Include nginx:1.12-alpine,php7.0,mysql:5.7.

Installation
------------

Clone from [myzero1/docke-lemp](https://github.com/myzero1/docker-lemp)

  ```
  git clone https://github.com/myzero1/docker-lemp.git
  ```

Setting by modify the docker-comose.yml
-----

- Seting the password of mysql

    ```
    - MYSQL_ROOT_PASSWORD=myzero1To123456
    ```

Usage
-----

- Start docker
    ```
    service docker start
    ```

- Build by docker-comose as following：
    ```
    docker-compose build
    ```

- Up by docker-comose as following：
    ```
    docker-compose up
    ```
OR run in backend
    ```
    docker-compose up -d
    ```

- Select containers
    ```
    docker-compose ps
    ```

- Log into the app container
    ```
    docker-compose exec php bash

    docker exec -it docker-lemp_php_1 bash   on docker for windows
    ```

- Using composer in php container
    ```
    docker-compose exec php bash

    composer -v
    ```

- Get the docker host IP address
    ```
    docker-machine env [machine name]
    ```

- More usefull commands
  - Stop containers
      ```
      docker-compose stop
      ```
   - Start containers
      ```
      docker-compose start
      ```
  - Restart containers
      ```
      docker-compose restart
      ```
  - Remve containers and images
      ```
      docker-compose rm
      ```
  - Add containers and images
      ```
      docker-compose up
      ```
      or
      ```
      docker-compose up -d
      ```
- using in docker-boxtool
    We will stor the db file to the linux vm of boxtool.We can upload/download from the linux vm by winscp/sftp
