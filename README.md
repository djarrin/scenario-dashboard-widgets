# scenario-dashboard-docker
A small docker instance with the [scenario widgets](https://github.com/city-of-baltimore/scenario-dashboard-widgets) as a submodule

## getting started

Note: Docker is required before beginning.

`git clone https://github.com/city-of-baltimore/scenario-dashboard-docker.git`

`cd scenario-dashboard-docker`

`git submodule update --init --recursive`

Create a developer account on [ArcGIS Online](https://arcgis.com)

Copy down the domain name after logic, this will be required for setting up the local dashbaord.

Navigate to the [ArcGIS Developer Dashboard](https://developers.arcgis.com/dashboard)

On the OAuth 2.0 tab, create a "New Application"

Copy the client id from the newly created application

Open config.json and paste the client id in:

`"appId": ""`

Check on the other config values. then copy the config into the widget directories.

`cp config.json volumes/widgets/scenario-dashboard`
`cp config.json volumes/widgets/scenario-database-config`


## Getting Set Up for local development

run `docker-compose up`

Navigate to https://localhost:3001

Copy the ArcGIS domain into the domain field

Copy the client id into the client id field

Login to ArcGIS online when prompted

## Creating the Dashboard app

1. Click "Create New" and choose "Blank Fullscreen".

2. Drag a map widget onto the screen.

3. Find the scenario dashboard widget and drag it onto the screen.

Note: It is recommended to position the map on the right of the screen and the dashboard widget on the left.

4. Click on the scenario dashboard widget. On the right side of the screen, there will be a "Content" tab. Click the dropdown that says "None", and select "Map" under "Current page".

5. Hit the disc icon to save and then Publish. Under the three dots menu, select "View published item".

## Contributing to this project

To start, read the documentation in the [scenario widgets](https://github.com/city-of-baltimore/scenario-dashboard-widgets) repository. This repository will use the same contribution guidelines, of creating an issue and checking out a new branch named after the issue. 

For submodule updates, the commit message should be "Widgets submodule update [current commit]".

You can find the current commit with `git diff volumes/widgets`.
