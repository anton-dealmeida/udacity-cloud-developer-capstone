# Udacity Capstone Project

> This project utilizes the projects built during the duration of the course.

This solution utilizes Amazon AWS as the Cloud Service provider and heavily depends on Serverless Framework.

Tools used:

- Serverless Framework
- NodeJS
- React

## Project structure

```
.
├── backend
│   ├── models
│   └── src
│       ├── auth
│       ├── businessLogic
│       ├── dataLayer
│       ├── lambda
│       │   ├── auth
│       │   ├── dynamoDb
│       │   ├── http
│       │   ├── s3
│       │   └── websocket
│       ├── models
│       └── requests
└── client
    ├── public
    └── src
        ├── api
        ├── auth
        ├── components
        └── types
```

## About the client directory

This directory contains the front end application. It's built with NodeJS using the React Library.

## About the backend directory

This directory contains the infrastructure code and code for spinning up the resources on Amazon AWS and deploying the backend idempotently.

## Getting started

### Backend

In the backend directory install npm packages.

```bash
    cd ./backend
    npm install
```

Install serverless globally for deployments.

```bash
    npm i -g serverless
```

Configure your Amazon credentials if not yet done.

### Frontend

```bash
    cd ./backend
    npm install
```

To run your frontend application use `npm run start`

## CI/CD

This repository automatically releases to AWS on commits.
