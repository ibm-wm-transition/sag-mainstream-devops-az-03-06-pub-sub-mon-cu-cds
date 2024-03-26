# Subscriber Microservice Development Run Configuration

## Quick start

- Obtain a valid Universal Messaging License and put it in the file `./config/UM/License/licence.xml`
  - Note that the path and file name must match exactly
- Obtain a valid Microservices Runtime license file
- copy `EXAMPLE.env` into `.env`
- edit the `.env` file as needed
- at the start time and whenever the database volume is destroyed, initialize the database with
  - `initDb.bat`
- start the project with `docker compose up`
- Start a designer instance and connect it to the main MSR port `http://localhost:${HOST_PORT_PREFIX}55`
  - Develop the needed functionality
  - Remember that packages are bind mounts, follow the example in `docker-compose.yml`
- You may observe UM using Enterprise Manager at `nsp://localhost:${HOST_PORT_PREFIX}90`
- You may observe the database contents by connecting a browser to `nsp://localhost:${HOST_PORT_PREFIX}80`
