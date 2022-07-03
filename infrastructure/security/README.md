<div align="center">
  <h1>Café Management Application Security</h1>
  <p>This application uses <strong>OAuth2</strong> mechanism for auth operations.</p>
</div>

<hr />

## Table Of Contents
- [Prerequisites](#prerequisites-anchor)
- [How To Initialize](#how-to-initialize-anchor)
- [How To Run](#how-to-run-anchor)


<a name="#prerequisites-anchor"></a>
## Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Keycloak 12.0.1](https://www.keycloak.org/downloads)
- [Postgres 12.1](https://www.postgresql.org/download/)


<a name="#how-to-initialize-anchor"></a>
## How To Initialize

`COMMAND_PARAMS="-Dkeycloak.migration.action=import -Dkeycloak.profile.feature.upload_scripts=enabled -Dkeycloak.migration.provider=singleFile -Dkeycloak.migration.file=/tmp/keycloak-config.json -Dkeycloak.import=/tmp/keycloak-config.json" docker-compose -f docker-compose.yml up -d`

<a name="#how-to-run-anchor"></a>
## How To Run

`docker-compose -f docker-compose.yml up -d`