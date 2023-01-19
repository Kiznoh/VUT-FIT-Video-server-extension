# VUT-FIT-Video-server-extension
VUT FIT Video server extension

## Instalation

To install the extension, visit [this website](https://lesson-titles-videoserver-fit-vut.cunt.cz/ext/ext.html) and click the install link. 

## Running the API server

### Using docker
To start the server, run 
```
docker compose up -d
```
To rebuild the container, run
```
docker compose build
```
Extension uses HTTPS to access the API server, some kind of reverse proxy or other solution is required.
The container exposes the API using HTTP to a docker network called `outside`.

## Updating the extension
The extension manifest specifies a update URL. It is avaible from the API server at `/ext/updates.json`.
