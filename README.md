# Oracle XE Docker

A simple usage example of Oracle Database Express Edition using Docker containers and docker-compose.

## Quick start

1. Specify the desired flavor of Oracle Database Express Edition through the `TAG` environment variable in `.env` (If not specified, it will default to version `18`).

   _A list of available editions is listed in the **Supported tags and respective Dockerfile links** section on [Dockerhub](https://hub.docker.com/r/gvenzl/oracle-xe)._

2. Edit your password settings in the `oracle.env` file. More information on the available environment variables [here](https://hub.docker.com/r/gvenzl/oracle-xe).
3. Download the image and spin up your container (Make sure your tag is correct if you are getting an error) by running

```sh
$ docker-compose up
```

4. Once you get the message **`DATABASE IS READY TO USE`** , you can connect by running the `sqlplus-connect.sh` script or through any GUI tool.

## Credits

Credits go to [gvenzl](https://github.com/gvenzl) for creating and maintaining the Dockerfiles for the different Oracle XE editions.
