# Intro

A lot of people doing the CS261 group project will be using a Django-React-Postgres stack.

However, figuring out containarisation for this can be a little tricky to get used to.

This repository provides a blank application using this stack, so any group can get started on their project.

# Usage

Ensure you have Docker installed. (Linux users may also have to install docker compose separately)

Windows users will have to install WSL2 (I recommend using the Ubuntu distro). They will also have to ensure [Docker is set up as shown](https://imgur.com/a/xcgPMLA)


To start up the system, run the command `docker compose up frontend`. This tells docker compose to set 'up' a service, and we specify the frontend. Since the frontend is set to depend on the backend and the database in the `docker-compose.yaml` file, all 3 services will be built.

The first time this command is run may take some time as generic images must be downloaded.

Eventually, all services should be up and running. 

To access the Django app, navigate to `localhost:8000`. For the React app, `localhost:3000`.

To safely close, try interrupting with Control-C, and running `docker compose down` after.

Sometimes, your issues might arise due to problems with cached images. You may want to try `docker container prune`

# Notes

All copyright remains with copyright holder. Majority of docker configurations taken from various online tutorials, assembled here by Michal Gagala with help from Joshua Fitzmaurice.

Note this repository is provided as-is, with no guarantee of adhering to relevant standards. We take no responsibility for any adverse effect or loss of marks due to mistakes in this repository or the README you are currently reading.
