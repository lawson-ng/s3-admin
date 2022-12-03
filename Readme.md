# Local Dashboard S3
Local dashboard S3 is a web-based tool for S3.

!["home"](./assets/home.png)

## Usage
#### Docker
```bash
docker pull abrahamlawson/local-dashboard-s3
```
**docker-compose** example: [link](./example/docker-compose.yml)


## Tech Stack
- BE: ExpressJS
- FE: ReactJS
- Monorepo (NPM workspace)

**Different ports used by the services the project spins up**
- 3000 - Web
- 3001 - Server/Api

## Source tree 🌲
```
.
├── Dockerfile
├── Readme.md
├── app <-- web
│   ├── README.md
│   ├── package.json
│   ├── public
│   ├── src
│   ├── tailwind.config.js
│   └── tsconfig.json
├── assets
│   └── home.png
├── docker-compose.yml
├── example
│   └── docker-compose.yml
├── package-lock.json
├── package.json
├── server <- server/api
│   ├── dist
│   ├── nodemon.json
│   ├── package.json
│   ├── src
│   └── tsconfig.json
├── shared
│   ├── constant
│   ├── dist
│   ├── index.ts
│   ├── interface
│   ├── package.json
│   └── tsconfig.json
├── todo.md
└── tsconfig.json
```

## API documentation
https://documenter.getpostman.com/view/16258208/2s8YswQXCC

## Dependencies

```

├── @typescript-eslint/eslint-plugin@5.43.0
├── @typescript-eslint/parser@5.43.0
├─┬ app@0.1.0 -> ./app
│ ├── @tailwindcss/forms@0.5.3
│ ├── @types/react-dom@18.0.9
│ ├── @types/react@18.0.25
│ ├── axios@1.2.0
│ ├── query-string@7.1.1`
│ ├── react-dom@18.2.0
│ ├── react-scripts@5.0.1
│ ├── react@18.2.0
│ ├── tailwindcss@3.2.4
│ └── typescript@4.9.3
├── concurrently@7.6.0
├── eslint@8.28.0
├── prettier@2.7.1
├─┬ server@1.0.0 -> ./server
│ ├── @aws-sdk/client-s3@3.213.0
│ ├── @types/express-fileupload@1.4.1
│ ├── @types/express@4.17.14
│ ├── @types/morgan@1.9.3
│ ├── @types/multer@1.4.7
│ ├── @types/node@18.11.9
│ ├── body-parser@1.20.1
│ ├── concurrently@7.6.0 deduped
│ ├── cors@2.8.5
│ ├── dotenv@16.0.3
│ ├── express-fileupload@1.4.0
│ ├── express@4.18.2
│ ├── morgan@1.10.0
│ ├── multer@1.4.5-lts.1
│ ├── nodemon@2.0.20
│ ├── pino@8.7.0
│ ├── ts-node@10.9.1
│ ├── tsconfig-paths@4.1.0
│ └── typescript@4.9.3 deduped
└── shared@1.0.0 -> ./shared

```
