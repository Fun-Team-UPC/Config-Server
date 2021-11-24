# Config-Server

#Upload to GCP
$ gcloud components update
$ gcloud version
$ gcloud auth login
$ gcloud config set project spring-boot-upc-api
$ gcloud init
$ gcloud services enable containerregistry.googleapis.com
$ gcloud auth configure-docker
$ docker image ls

$ docker tag ilanguage-config-server-fas:latest gcr.io/ilanguage-fas/ilanguage-config-server-fas:latest
$ docker tag ilanguage-registry-service-fas:latest gcr.io/ilanguage-fas/ilanguage-registry-service-fas:latest
$ docker tag ilanguage-api-gateway-fas:latest gcr.io/ilanguage-fas/ilanguage-api-gateway-fas:latest
$ docker tag demo-spring-boot:latest gcr.io/spring-boot-upc-api/demo-spring-boot:latest

$ docker push gcr.io/ilanguage-fas/ilanguage-config-server-fas:latest
$ docker push gcr.io/ilanguage-fas/ilanguage-registry-service-fas:latest
$ docker push gcr.io/ilanguage-fas/ilanguage-api-gateway-fas:latest
$ docker push gcr.io/spring-boot-upc-api/demo-spring-boot:latest
