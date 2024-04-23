## Running the Server

To run the server, use the following command:

```bash
poetry install. # this is optional after the first install
poetry run eidolon-server resources/
```

If you wish to run the server without MongoDB, include the `-m local_dev` flag:

```bash
poetry install. # this is optional after the first install
poetry run eidolon-server resources/ -m local_dev
```

## Running the UI

To run the ui on mac, use the following command from the root project directory:

```bash
docker run -e EIDOLON_APP_REGISTRY_OVERRIDE="$(< eidolon-apps.json)" -p 3000:3000 eidolonai/webui:test_apps_override
```
