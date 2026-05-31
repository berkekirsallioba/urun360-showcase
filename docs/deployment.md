# Deployment

Ürün360 is designed for local or internal server deployment.

## Windows Service Model

The application runs as a Windows Service on the hosting machine. This service hosts both the backend API and the frontend static files.

The goal is to allow the application to start automatically when Windows starts.

## Local / Server Installation

Typical installation targets:

- Local cashier computer
- Internal server
- Back-office machine
- Store network server

## Browser-Based Access

Users access Ürün360 from a browser. The application is not distributed as a traditional desktop application for end users.

Example URLs:

```text
http://localhost:8890/display
http://SERVER-IP:8890/display
http://SERVER-IP:8890/operator
http://SERVER-IP:8890/admin
```

## Public IP Note

Public IP access is not the primary deployment target. If external access is required, firewall, router forwarding, HTTPS, authentication, and access restriction must be reviewed separately.

## Executable Note

If an executable file exists in the deployment package, it is used only as the server-side application host. End users access the application through a browser.
