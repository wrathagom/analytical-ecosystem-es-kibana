# Personal Analytical Ecosystem: Elasticsearch and Kibana

Thanks for coming to check out my [analytical ecosystem](https://calebmkeller.com/building-a-personal-analytical-ecosystem/)! This repo adds Elasticsearch and Kibana to the same Docker network as the other tools in the ecosystem. You can run it with other components or independantly.

## Installation

Getting started is easy, if you already have Docker and docker-compose installed. If you don't take care of that first:

 - [Install Docker](https://docs.docker.com/get-docker/)
 - [Install docker-compose](https://docs.docker.com/compose/install/)

After that it's as simple as:

 - Clone this repo - `git clone https://github.com/wrathagom/analytical-ecosystem-es-kibana.git`
 - Move to the new folder - `cd analytical-ecosystem-es-kibana`
 - Docker compose up - `docker-compose up -d && docker-compose logs -f`

## Access

Elasticsearch can take a moment to start up. But once it is reasy you can access Kibana at http://localhost:5601 and the Elasticsearch API at http://localost:9200

## Updating

This repo is still changing frequently. To update run the below commands:

```
git pull
docker-compose down
docker-compose build
docker-compose up -d
docker-compose logs -f
```

This pulls the latest repo info from Github, shuts down the services, updates the images, and starts everything back up again.
