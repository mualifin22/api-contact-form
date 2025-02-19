# api-contact-form
Build and Run Application

Before containerizing the application with Docker, it’s important to build and run it locally to ensure everything works as expected.
Installing Dependencies

Ensure that all necessary Go dependencies are installed. Run the following command to download the dependencies specified in go.mod:

```sh
go mod tidy
```
This command updates the go.sum file with the checksums of the dependencies.
Building the Application

Compile the Go application by running

# this will generate binary file with filename following folder project name (api-contact-form)
go build 

or 

# if you want ot create binary with custom filename you can use -o parameter
go build -o api-contact-form .

This command builds the application and outputs an executable named main.
Running the Application

Start the application locally using:

./api-contact-form


💡

Confirm that MariaDB is up and running, ensure all required databases have been created, and check that your environment settings properly support database connections.
Step 12: Testing the API

With the application running inside Docker containers, you can now test the API endpoints using tools like Postman, cURL, or Insomnia.
Health Check

Verify that the API is operational.

curl --location 'http://localhost:8080/health'
