# SPARKR SERVER

The project is generated by [LoopBack](http://loopback.io).

## Configuration

### OSX

* Edit your ~/.bashprofile file and set the following environment variables:
```bash
export MONGODB_HOST='cluster0-shared-cloud.net'
export MONGODB_PORT=27017
export MONGODB_URL='mongodb://username:password@cluster0-shared-cloud.net:27017/collection?replicaSet=Cluster0-shared-0&authSource=admin&ssl=true'
export MONGODB_DATABASE='collection'
export MONGODB_USER='username'
export MONGODB_PASSWORD='password'
```

* The environment variables match the variables used in the '~/server/datasources.json' configuration file
```text
    "host": "${MONGODB_HOST}",
    "port": "${MONGODB_PORT}",
    "url": "${MONGODB_URL}",
    "database": "${MONGODB_DATABASE}",
    "user": "${MONGODB_USER}",
    "password": "${MONGODB_PASSWORD}",
```

## Generate a Swagger or Open API Specification 

See [Loopback API Definition Generator](https://loopback.io/doc/en/lb3/API-definition-generator.html).

## Add API Management with API Key to Server

## Send a Request from Client

```bash
curl --request GET \
  --url 'https://sparkrapi.mybluemix.net/api/Members?filter=REPLACE_THIS_VALUE' \
  --header 'accept: application/json' \
  --header 'x-ibm-client-id: apikey'
```

