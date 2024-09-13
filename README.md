# starters-2024-hoppscotch
Repo with code to deploy Hoppscotch locally using Docker compose



Requirements:
- Node.js
- npm
- pnpm
- Docker
=> install instructions can be found on https://docs.hoppscotch.io/documentation/self-host/community-edition/prerequisites


Clean install from the repo:\
=> download/clone code from repo\
=> go to the folder where the code is located in the terminal\
=> run docker compose up in terminal\
=> The backend container will fail to start and the error message “Database migration not found. Please check the documentation for assistance: https://docs.hoppscotch.io/documentation/self-host/community-edition/install-and-build#running-migrations” will appear in between the logs\
=> execute docker compose run --entrypoint sh hoppscotch-backend in terminal\
=> execute pnpx prisma migrate deploy in container\
=> open browse, navigate to http://localhost:3100/ and setup admin access. First person to login get admin rights\
=> use Hopscotch service on http://localhost:3000/\
