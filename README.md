# starters-2024-hoppscotch
Repo with code to deploy Hoppscotch locally using Docker compose


<h3>Requirements:</h3>
- Node.js
- npm
- pnpm
- Docker
=> install instructions can be found on https://docs.hoppscotch.io/documentation/self-host/community-edition/prerequisites

<h3>Clean install from the repo:</h3>
=> download/clone code from repo<br>
=> go to the folder where the code is located in the terminal<br>
=> run docker compose up in terminal<br>
=> The backend container will fail to start and the error message “Database migration not found. Please check the documentation for assistance: https://docs.hoppscotch.io/documentation/self-host/community-edition/install-and-build#running-migrations” will appear in between the logs
=> execute docker compose run --entrypoint sh hoppscotch-backend in terminal<br>
=> execute pnpx prisma migrate deploy in container<br>
=> open browse, navigate to http://localhost:3100/ and setup admin access. First person to login get admin rights<br>
=> use Hopscotch service on http://localhost:3000/<br>
