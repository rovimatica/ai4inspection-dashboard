# AI4INSPECTION Dashboard

Dashboard to monitorize the information provided by the AI4INSPECTION automated food quality control system.

## Install

To install this component, docker and FIWARE must be properly installed and functioning without issues.

You can find a script to install both in the following repository: https://gitlab.lst.tfo.upm.es/shop4cf/fiware-deployment.

Clone or download this repo on your system. It contains a docker image ready to use. To start the image use

```
docker load -i ai4inspection-dashboard.tar
docker compose up -d

```

You can access the dashboard by going to http://localhost:3001/d/ai4inspection/ai4inspection.

The dashboar credentials are

    User: user
    Password: user

## Custom configuration

The docker image is prepared to connect to FIWARE over the fiware_default network. If your FIWARE instance is on a different network, you must rename the network name in docker-compose.yml.

The image uses the local port 3001. You can change the port in docker-compose.yml to use a different one.