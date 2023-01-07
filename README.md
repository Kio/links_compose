# Links

The application allows you to find all links on a specified URL, including nested links up to a depth of 3.

It consists of a [React frontend](https://github.com/Kio/links_frontend) and a [Django backend](https://github.com/Kio/links_backend).

## Requirements

To set up the application, you will need to clone the relevant repositories into the `frontend` and `backend` folders:

```
git clone https://github.com/Kio/links_compose.git
cd links_compose
git clone https://github.com/Kio/links_frontend.git frontend
git clone https://github.com/Kio/links_backend.git backend
```
Also you will need [docker-compose](https://docs.docker.com/compose/install/) tool.

## Development

Frontend will be run with react-scripts, backend with default Django web server. Hot swap for code will be available for both. Command to start:

`docker-compose up`

## Production

Frontend will be compiled and served with nginx. Backend will be served using nginx and gunicorn serving as the reverse proxy. To start the application, use the provided command:

`docker-compose -f docker-compose-prod.yml up`
