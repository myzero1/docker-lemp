docker-lemp
========================
This is a lenmp evn builded by docker-compose.Include nginx:1.12-alpine,php7.0,mysql:5.7.

Installation
------------

Clone from [myzero1/docke-lemp](https://github.com/myzero1/docker-lemp)

  ```
  git clone https://github.com/myzero1/docker-lemp.git
  ```

Setting
-----

- Go to env dir and copy .env.dist to .env

    ```
    cd env
    cp .env.dist .env
    ```

- Go to env dir and copy conf.dist to conf

    ```
    cd env
    cp conf.dist conf
    * you can edit the COMPOSE_PROJECT_NAME,if you want more env
    ```


Usage
-----

- Go to env dir
    ```
    cd env
    ```

- Build env by docker-comose as following：
    ```
    docker-compose build
    ```

- Up env by docker-comose as following：
    ```
    docker-compose up
    ```
OR run in backend
    ```
    docker-compose up -d
    ```

- Log into the app container
    ```
    docker-compose exec app bash
    
    docker exec -it env_app_1 bash   on docker for windows
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
      docker-compose up
      ```
