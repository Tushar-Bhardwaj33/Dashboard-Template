# React Admin Dashboard

A responsive and feature-rich admin dashboard built with React, Material-UI, and various other libraries. This dashboard provides a comprehensive interface for managing and visualizing data, making it suitable for various applications, including analytics, project management, and more.

## Features

- **Data Tables**: Utilize Material-UI Data Grid for customizable and interactive data tables.
- **Forms**: Implement forms with Formik and Yup for validation, allowing users to input and manage data easily.
- **Charts**: Visualize data with Nivo charts, including bar, pie, line, and geographical charts.
- **Multi-language Support**: Enable users to interact with the dashboard in multiple languages.
- **Responsive Design**: Fully responsive layout that works seamlessly on both desktop and mobile devices.
- **Dark/Light Mode**: Toggle between dark and light themes for user preference.
- **Routing**: Use React Router for navigation between different sections of the dashboard.

## Technologies Used

- **React**: JavaScript library for building user interfaces.
- **Material-UI**: React components that implement Google's Material Design.
- **Formik**: Library for building forms in React with ease.
- **Yup**: Schema builder for value parsing and validation.
- **Nivo**: Data visualization library for creating beautiful charts.
- **React Router**: Declarative routing for React.js applications.
- **Axios**: Promise-based HTTP client for making API requests.

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