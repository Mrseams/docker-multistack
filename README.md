# 📁 Structure du projet avec fichiers réels (archive prête)

angular/
├── spa/
│ ├── Dockerfile
│ ├── .dockerignore
│ └── angular-app/
│ ├── angular.json
│ ├── package.json
│ ├── tsconfig.json
│ └── src/index.html
├── ssr/
│ ├── Dockerfile
│ ├── .dockerignore
│ └── angular-ssr-app/
│ ├── angular.json
│ ├── package.json
│ ├── tsconfig.server.json
│ └── src/index.html

express/
├── Dockerfile
├── .dockerignore
└── express-app/
├── package.json
└── index.js

nestjs/
├── Dockerfile
├── .dockerignore
└── nest-app/
├── package.json
├── tsconfig.json
└── src/main.ts

oracle-api/
├── Dockerfile
├── .dockerignore
└── oracle-api/
├── package.json
└── index.js

nginx/
├── Dockerfile
├── default.conf
├── waf/
│ └── modsecurity.conf

📄 docker-compose.yml
📄 README.md
