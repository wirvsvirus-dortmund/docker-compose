# docker-compose

Deployment using docker-compose


1. Have this repo checked out in the same directory as frontend and backend, e.g. like this
    ```
    $ mkdir supermarkt && cd supermarkt
    $ git clone https://github.com/wirvsvirus-dortmund/frontend 
    $ git clone https://github.com/wirvsvirus-dortmund/backend 
    $ git clone https://github.com/wirvsvirus-dortmund/docker-compose
    $ cd docker-compose
    ```
1. Copy the env-template to .env and fill in the necessary values
1. run 
    ```
    $ docker-compose up --build
    ```

1. Visit http://localhost:8080
