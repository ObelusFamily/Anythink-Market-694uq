# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_


## Install Docker
Docker can be installed via this link: https://docs.docker.com/get-docker/
It is required to run the frontend, backend, and database for the the Anyythink app.
Once docker is installed you can run `docker -v` & `docker-compose -v` to verify that it is up and running.


## Start up the project
Navigate to the project root directory (where you cloned the Anythink repo to) and run `docker-compose up`. 
This will startup the frontend, backend, and database. It wwill take a few moments the first time you run this
as your system will need to download all the required files.

After your computer has finished downloading the required files you will begin to see a series of logs being written to the console (likely just from momgodb for now).

To make sure the backend is up and running, navigate to http://localhost:3000/api/ping . You should see `{"msg":"Pong! Seems like Everythink is working, great job!"}` if the backend is up and running.

To make sure the frontend is up and running, navigate to http://localhost:3001/register . You should see a registration page. Register an account to move to the next step.

For the remaining quests on your journey to developer stardom, make sure to run all the scripts on at least one of the containers that were created in docker via the previous steps.
Commands can be run against a running container using `docker exec`
