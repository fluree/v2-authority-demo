# Fluree Authority Demo

## How to Use

We include a `docker-compose.yml` file to make it easy to run the Fluree Authority Demo. To start the demo, run the following command from the project directory:

```bash
docker compose up -d && sleep 10 && npm i && node index.js
```

> I only include the `sleep 10` because the Fluree server takes a few seconds to start up, and if the NPM packages are already installed, then the node script will run before the Fluree server is ready

If you want to reset & re-run the script, make sure to fully delete the container, otherwise the container will restart with the same data state.

```bash
docker compose down && docker compose up -d && sleep 10 && node index.js
```
