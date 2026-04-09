## Droplet

1. create a droplet
2. ubuntu, smol
3. reserve ip
4. setup ssh

## Docker

1. on the droplet, [install docker](https://docs.docker.com/engine/install/ubuntu/)

## Code

1. clone this repo on droplet
2. make env vars
    ```
    cp .env.example .env
    ```
3. use `nano` or `vi` or something to update the `.env` file
4. start it up! and se if it's working
    ```
    docker compose up --build
    ```
5. <kbd>ctrl</kbd>+<kbd>C</kbd> to kill it
6. once it's working good, start it as a daemon
    ```
    docker compose up -d --build
    ```