# starters-2024-hoppscotch

Repo with code to deploy Hoppscotch locally using Docker compose

## Requirements

- Node.js
- npm
- pnpm
- Docker

> install instructions can be found on https://docs.hoppscotch.io/documentation/self-host/community-edition/prerequisites

## Clean install from the repo

- clone code from repo, `main` branch
- navigate to the folder where the code is located in the terminal
- run `docker compose up` in terminal
- the backend container will fail to start and the error message `Database migration not found. Please check the documentation for assistance: https://docs.hoppscotch.io/documentation/self-host/community-edition/install-and-build#running-migrations` will appear in between the logs
- execute `docker compose run --entrypoint sh hoppscotch-backend` in the terminal
- you'll enter the docker container
- execute `pnpx prisma migrate deploy` in the container
- open browser navigate to [http:localhost:3100/](http:localhost:3100/) and setup admin access
    - first person to login gets admin rights
- use Hopscotch service on [http:localhost:3000/](http:localhost:3000/)