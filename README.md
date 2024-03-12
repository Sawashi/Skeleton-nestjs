## Description <!-- omit in toc -->

NestJS REST API boilerplate for typical project

[Full documentation here](/docs/readme.md)

Demo: <https://nestjs-boilerplate-test.herokuapp.com/docs>

Frontend (React, Next.js): <https://github.com/brocoders/extensive-react-boilerplate>

## How to run:
- Install Postgres: https://www.postgresql.org/download/
- Install pgadmin: https://www.pgadmin.org/download/
- Install docker: https://docs.docker.com/desktop/install/windows-install/
- Add .env file: https://drive.google.com/file/d/1niDLMgkuVUqXR7mi4YdXpDSirI1lyBLi/view?usp=sharing
- Open docker desktop (if you have errors with docker, delete volumes + container + images + builds and try again)
- Run
  ```
  npm install
  ```
  ```
  docker compose up -d postgres adminer maildev
  ```
  ```
  npm run migration:run
  ```
  ```
  npm run seed:run:relational
  ```
  ```
  npm run start:dev
  ```
* Note 1: If you have error dont exists database, please delete all things in docker then connect again.
* Note 2: If you ran into error cannot login to db, please use this tutorial to change your password:
https://www.postgresqltutorial.com/postgresql-administration/postgresql-reset-password/
## Links
- Main links for apis: http://localhost:3000
- Swagger (API docs): http://localhost:3000/docs
- Adminer (client for DB): http://localhost:8080
  ![Screenshot 2024-03-12 115902](https://github.com/Sawashi/Skeleton-nestjs/assets/92447748/4c849b74-eb72-4791-81a7-ae5fdcd0b042)
  * Note: the password is "secrect"
- Maildev: http://localhost:1080

## Features

- [x] Database. Support [TypeORM](https://www.npmjs.com/package/typeorm) and [Mongoose](https://www.npmjs.com/package/mongoose).
- [x] Seeding.
- [x] Config Service ([@nestjs/config](https://www.npmjs.com/package/@nestjs/config)).
- [x] Mailing ([nodemailer](https://www.npmjs.com/package/nodemailer)).
- [x] Sign in and sign up via email.
- [x] Social sign in (Apple, Facebook, Google, Twitter).
- [x] Admin and User roles.
- [x] Internationalization/Translations (I18N) ([nestjs-i18n](https://www.npmjs.com/package/nestjs-i18n)).
- [x] File uploads. Support local and Amazon S3 drivers.
- [x] Swagger.
- [x] E2E and units tests.
- [x] Docker.
- [x] CI (Github Actions).


