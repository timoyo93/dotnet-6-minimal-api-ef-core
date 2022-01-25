## .Net 6 Minimal API with EF Core

This is a sample projcet to showcase, how a minimal API in .Net 6 is set up.
For data storage during runtime, EF Core with an In Memory Database is used

## Docker

In order to run the API inside of a docker container, you need to build the image first:

1. First you need to change into the `src/` directory with your Terminal
2. Run the following command: <br> `docker build . -t pizza-store:latest`

Once the build has finished you can run the container with with command:

`docker run -i --rm -p 8080:80 pizza-store:latest`

Now the app should be running and you can call the API via http://localhost:8080/ or use the Swagger UI via http://localhost:8080/swagger/
