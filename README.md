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
=> run <strong>docker compose up</strong> in terminal<br>
=> The backend container will fail to start and the error message <strong>“Database migration not found. Please check the documentation for assistance: https://docs.hoppscotch.io/documentation/self-host/community-edition/install-and-build#running-migrations”</strong> will appear in between the logs
=> execute <strong>docker compose run --entrypoint sh hoppscotch-backend</strong> in terminal<br>
=> execute <strong>pnpx prisma migrate deploy in container</strong><br>
=> open browse, navigate to http://localhost:3100/ and setup admin access. First person to login gets admin rights<br>
=> use Hopscotch service on http://localhost:3000/<br>
