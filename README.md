# Tailwind + Angular + Nest + Node + MySQL

Full-stack starter workspace with:

- `angular-client`: Angular 21 frontend (with Tailwind dependency installed)
- `nest-server`: NestJS 11 backend (Node/Express)

## Project Status

This repository currently contains framework starter templates.

- Frontend: default Angular starter page
- Backend: default NestJS `GET /` endpoint returning `Hello World!`
- Database: MySQL is not configured in code yet

## Workspace Structure

```text
.
|-- angular-client/
|-- nest-server/
`-- README.md
```

## Prerequisites

- Node.js 20+ (recommended)
- npm 10+
- MySQL 8+ (optional for now, required when DB integration is added)

## Installation

Install dependencies in each app:

```bash
cd angular-client
npm install

cd ../nest-server
npm install
```

## Run In Development

Run backend (NestJS):

```bash
cd nest-server
npm run start:dev
```

Backend default URL:

- `http://localhost:3000`

Run frontend (Angular):

```bash
cd angular-client
npm start
```

Frontend default URL:

- `http://localhost:4200`

## Build

Frontend build:

```bash
cd angular-client
npm run build
```

Backend build:

```bash
cd nest-server
npm run build
```

## Test

Frontend tests:

```bash
cd angular-client
npm test
```

Backend tests:

```bash
cd nest-server
npm test
```

Backend e2e tests:

```bash
cd nest-server
npm run test:e2e
```

## Current API

NestJS exposes:

- `GET /` -> `Hello World!`

## Notes On MySQL

The repository name includes MySQL, but DB integration is not implemented yet.

Planned next step is to add:

- a database module/ORM (e.g., TypeORM or Prisma)
- environment variables for DB connection
- migration workflow
- sample entity/module CRUD

## Useful Scripts

`angular-client/package.json`

- `npm start` -> `ng serve`
- `npm run build` -> production build
- `npm test` -> Angular unit tests

`nest-server/package.json`

- `npm run start:dev` -> watch mode
- `npm run build` -> compile Nest app
- `npm test` -> unit tests
- `npm run test:e2e` -> e2e tests

## License

Each subproject currently follows its generated starter defaults.