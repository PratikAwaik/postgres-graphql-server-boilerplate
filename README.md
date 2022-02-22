# postgres-graphql-server-boilerplate

Server side boilerplate for PostgreSQL and GraphQL with Sequelize, Apollo and Umzug (for migrations).

### Folder structure

|-- migrations
|   `-- 2022_02_22_01_initialize_user.js
|-- models
|   |-- index.js
|   `-- user.js
|-- resolvers
|   |-- index.js
|   |-- query.js
|   `-- user.js
|-- typeDefs
|   |-- index.js
|   |-- query.js
|   `-- user.js
`-- util
    |-- config.js
    |-- db.js
    `-- rollback.js
|-- context.js
|-- index.js

### Connect your database
- Create a `.env` file in the root directory
- Add `PROD_DATABASE_URL` for production and `DEV_DATABASE_URL` for development purposes.
- Additionally, all the config would go into `util/config.js` 

### Naming migrations
The way migration is named here is -  `YYYY_MM_DD_<INDEX>_<NAME OF MIGRATION>`.

### Defining relationships between tables
For defining relationships between tables, use `models/index.js`

