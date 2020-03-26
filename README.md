# docker-compose [![Build Status](https://travis-ci.com/wirvsvirus-dortmund/docker-compose.svg?branch=master)](https://travis-ci.com/wirvsvirus-dortmund/docker-compose)

1. Have this repo checked out in the same directory as frontend and backend, e.g. like this
    ```
    $ mkdir supermarkt && cd supermarkt
    $ git clone https://github.com/wirvsvirus-dortmund/frontend 
    $ git clone https://github.com/wirvsvirus-dortmund/backend 
    $ git clone https://github.com/wirvsvirus-dortmund/docker-compose
    $ cd docker-compose
    ```
1. Copy the env-template to .env and fill in the necessary values

## Developing


1. Start the backend in the backend directory using 
    ```
    $ FLASK_DEBUG=true poetry run flask run
    ```

1. Start the frontend in the frontend directory

    ```
    $ npm run serve
    ```

1. Start the nginx coupling them together using
    ```
    $ docker-compose up -d nginx-dev
    ```



## Deployment


1. run 
    ```
    $ docker-compose up -d --build frontend backend database
    ```

1. Visit http://localhost:8080
