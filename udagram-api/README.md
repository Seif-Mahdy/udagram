# Udagram API

A Nodejs API that serves as the backend for the Udagram App

## To run the app locally

### Create your local DB

Create a Postgres DB instance

### Running the API

1. Clone the repo
2. Navigate to the "udagram-api" or from the cmd `cd udagram-api`
3. Run `npm i`
4. Create `.env` file with the environment variables as in the [ENVEXAMPLE](./ENVEXAMPLE) file
5. Run `npm run dev`

### App dependencies

* `aws-sdk`
* `bcryptjs`
* `body-parser`
* `cors`
* `dotenv`
* `email-validator`
* `express`
* `jsonwebtoken`
* `pg`
* `reflect-metadata`
* `sequelize`
* `sequelize-typescript`

### Available commands

* "start": Builds and serves your app (JS)
* "tsc": transpile the TS code to JS
* "dev": Builds and serves your app (TS)
* "prod": Builds and serves your app (JS)
* "clean": Removes the build files
* "deploy": deploy the app to AWS EB
* "build": Compiles the app into an output directory
