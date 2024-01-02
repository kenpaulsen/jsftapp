# Maven / Docker wrapper to help bootstap a containerized JSFT project.

To use this project, you will need to checkout subprojects for the actual content and update the `Dockerfile` to match. By default, it expects 3 sub-projects:
* app -- A directory containing a `webapp` folder for the root of a webapp, and normal java project w/ a jar file target. Both will be added via Docker.
* jsft -- Checkout via: git clone git@github.com:kenpaulsen/jsft.git
* freya -- If you have this primefaces theme, otherwise change to a theme you'd like to use (change `Dockerfile` as well).

## Docker Build
See [README-Docker.md](README-Docker.md) for details, but at a high level (for now):

### Build
1. mvn clean install
1. docker compose down
1. docker compose build

### Run
1. docker compose build

