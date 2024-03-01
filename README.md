# scenario-dashboard-docker
A small docker instance with the scenario widgets as a submodule

`git clone git@github.com:city-of-baltimore/scenario-dashboard-docker.git`

`cd scenario-dashboard-docker`

`git pull --recurse-submodules`

# Getting Set Up for local development

run `docker-compose up`

Navigate to https://localhost:3001

To login:

Create a developer account on arcgis.com

On the login screen, copy the domain that you are redirected to on login, paste it into the domain field

Navigate to https://developers.arcgis.com/

On the OAuth 2.0 tab, create a "New Application"

Copy the client id from the newly created application, and paste it into client id

