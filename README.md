# python-web-api-bottle-basic-auth-ssl-sqlserver-pop

## Description
Creates an api of `pop` for a bottle project.
Has the ability to query by parameters.

Remotely tested with *testify*, the ssl is not verified.

Requires basic authentication for endpoints.

| username | password |
| -------- | -------- |
| *user* | *pass* |

## Tech stack
- python
  - bottle
  - sqlalchemy
  - testify
  - requests
- mssql

## Docker stack
- python:latest
- mcr.microsoft.com/mssql/server:2017-CU17-ubuntu

## To run
`sudo ./install.sh -u`
- Get all pops: https://localhost/pop
  - Schema id, name, and color
- CRUD opperations
  - Read: https://localhost/pop/<id> -u 'user:pass'

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`
