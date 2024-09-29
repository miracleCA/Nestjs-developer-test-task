## Description
Based on the test/assessment requirements, this is a RESTful API service using NestJS with TypeScript that supports user authentication (standard and biometric), registration, and utilizes Prisma as the ORM. The API is exposed through GraphQL.

### **Requirements**
This test project matches all the needed requirements except from that of biometric which was already listed to be optional as I also didn't list it as part of the authentication due to time and variances. Secondly I added hashedRefreshToken in the <a href="/prisma/schema.prisma">Model</a> so as to allows the user to have short-lived access tokens without having to collect credentials every time one expires. Thirdly, I used <a href="/docker-compose.yml">Docker</a> to manage a local containerized database. Aside the above mentioned, there's no other differences as every other aspect of the project was implemented strictly based on the requirements.

There's a .env file inside the parent folder which has all the enviroment variables required for this project.

The GraphQL schema file is found inside the <a href="/src/">src</a> folder as it can be used to test the API endpoints.


## Installation

```bash
$ npm install
```
## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## To contact me

Developer - [Miracle Chukwuebuka Anyiam](https://www.linkedin.com/in/chukwuebuka-miracle-anyiam-879a2b177)
