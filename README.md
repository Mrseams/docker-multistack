# Docker Multi-Stack Project

This project is a multi-container application stack using Docker Compose. It includes:

- **Angular SPA** (Single Page Application)
- **Angular SSR** (Server-Side Rendering)
- **NestJS API** (Node.js backend)
- **Express App** (Node.js minimal API)
- **Oracle Node API** (Sample Node.js API)
- **NGINX** (Reverse proxy for all services)

## Project Structure

```
angular/
  spa/         # Angular Single Page Application
  ssr/         # Angular Server-Side Rendering
express/
  express-app/ # Express.js API
nestjs/
  nestjs-api/  # NestJS API
oracle-node-api/
  oracle-api/  # Oracle Node API
nginx/         # NGINX reverse proxy config
```

## Prerequisites

- [Docker](https://www.docker.com/products/docker-desktop) & [Docker Compose](https://docs.docker.com/compose/install/) installed

## How to Start the Project

1. **Clone the repository** (if you haven't already):

   ```powershell
   git clone <your-repo-url>
   cd docker-multistack
   ```

2. **Build and start all services:**

   ```powershell
   docker compose up --build
   ```

   This will build and start all containers defined in `docker-compose.yml`.

3. **Access the applications:**

   - **SPA:** http://localhost/
   - **SSR:** http://localhost/ssr/
   - **NestJS API:** http://localhost/api/
   - **Express:** http://localhost/express/
   - **Oracle API:** http://localhost/oracle/

   All traffic is routed through NGINX (http://localhost/).

4. **Stop the stack:**
   ```powershell
   docker compose down
   ```

## Service Details

- Each service has its own `DockerFile` and source code in its respective folder.
- NGINX reverse proxy is configured in `nginx/default.conf`.
- Modify or extend each service as needed for your use case.

## Development

- For local development of individual services, refer to the README in each service's folder (e.g., `angular/spa/README.md`, `nestjs/nestjs-api/README.md`).
- You can run and test each service independently using their respective instructions.

## License

This project is open source and available under the MIT License.
