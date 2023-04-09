# Roxabi !

Part of Roxabi framework, Blueprint modules to deploy complete application with :

-   **Front end :**
    -   **next js**
-   Back end
    -   node js
-   IAM :
    -   To be define
-   Database :
    -   Prisma
-   ELK :
    -   To be define
-   Event / notification :
    -   To be define
-   Webmail
    -   To be define
-   CI / CD :
    -   To be define
-   Automated test :
    -   To be define

## Frond end BluePrint

Blueprint modules to deploy complete application with :

-   Front end :
    -   next js
-   Back end
    -   node js
-   IAM :
    -   To be define
-   Database :
    -   Prisma
-   ELK :
    -   To be define
-   Event / notification :
    -   To be define
-   Webmail
    -   To be define
-   CI / CD :
    -   To be define
-   Automated test :
    -   To be define

## How to start

Optionally,

```bash
# Go in app folde
cd next-app
#Run `npm install`  to generate a lockfile.
npm install
```

It is recommended to commit a lockfile to version control. Although the example will work without one, build errors are more likely to occur when using the latest version of all dependencies. This way, we're always using a known good configuration to develop and run in production.

### Development

First, run the development server:

```bash
# Create a network, which allows containers to communicate
# with each other, by using their container name as a hostname
docker network create my_network

# Build dev
docker-compose -f docker-compose.dev.yml build

# Up dev
docker-compose -f docker-compose.dev.yml up
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

### Production

```bash
# Create a network, which allows containers to communicate
# with each other, by using their container name as a hostname
docker network create my_network

# Build prod
docker-compose -f docker-compose.prod.yml build

# Up prod in detached mode
docker-compose -f docker-compose.prod.yml up -d
```

Open [http://localhost:3000](http://localhost:3000).

## Benefits of Docker Compose

-   Develop locally without Node.js or TypeScript installed
-   Easy to run, consistent development environment across macOS, Windows, and Linux teams
-   Run multiple Next.js apps, databases, and other microservices in a single deployment
-   Easy configuration with YAML files

## Prerequisites

Install [Docker Desktop](https://docs.docker.com/get-docker) for Mac, Windows, or Linux. Docker Desktop includes Docker Compose as part of the installation.

## Useful commands

```bash
# Stop all running containers
docker kill $(docker ps -aq) && docker rm $(docker ps -aq)

# Free space
docker system prune -af --volumes
```
