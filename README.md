# postgres-12beta3-alpine-ap_pgutils

A variant of [postgres:12-beta3-alpine](https://hub.docker.com/_/postgres), with the [ap_pgutils](https://github.com/Apsalar/ap_pgutils) extension included.

This uses [jaredreisinger/postgres-12beta3-alpine-dev](https://hub.docker.com/r/jaredreisinger/postgres-12beta3-alpine-dev) to build the extension, then copies it into a clean [postgres:12-beta3-alpine](https://hub.docker.com/_/postgres) image.

## Usage

Once you have PostgreSQL spun up, use `CREATE EXTENSION ap_pgutils;` to get access to the ap_pgutils functions.
