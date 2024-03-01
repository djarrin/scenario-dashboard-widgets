# scenario-dashboard-docker
A small docker instance with the [scenario widgets](https://github.com/city-of-baltimore/scenario-dashboard-widgets) as a submodule

## getting started

`git clone git@github.com:city-of-baltimore/scenario-dashboard-docker.git`

`cd scenario-dashboard-docker`

`git pull --recurse-submodules`

Create a developer account on [ArcGIS Online](https://arcgis.com)

Copy down the domain name after logic, this will be required for setting up the local dashbaord.

Navigate to the [ArcGIS Developer Dashboard](https://developers.arcgis.com/dashboard)

On the OAuth 2.0 tab, create a "New Application"

Copy the client id from the newly created application

Open config.json and paste the client id in for appId

`cp config.json volumes/widgets/scenario-dashboard`
`cp config.json volumes/widgets/scenario-database-config`


## Getting Set Up for local development

run `docker-compose up`

Navigate to https://localhost:3001

Copy the ArcGIS domain into the domain field

Copy the client id into the client id field

Login to ArcGIS online when prompted


