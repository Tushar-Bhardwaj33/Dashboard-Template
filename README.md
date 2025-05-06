# Dashboard-Template
Made a dashboard template for data visulisation | React, Material UI, Data Grid, Light & Dark Mode

## Running with Docker

This project includes Docker and Docker Compose support for easy setup and deployment.

- **Node.js version:** 22.13.1 (as specified in the Dockerfile)
- **Exposed port:** 5000 (the dashboard will be available at http://localhost:5000)
- **No environment variables are required by default** (uncomment the `env_file` line in `docker-compose.yml` if you add a `.env` file)

### Build and Run

To build and start the dashboard app using Docker Compose:

```sh
docker compose up --build
```

This will build the React app and serve the static build using the `serve` package inside the container.

- The app runs as a non-root user for security.
- No external services or persistent volumes are required.

---
