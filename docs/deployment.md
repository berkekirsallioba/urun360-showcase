# Deployment Overview

Ürün360 follows a local / server-first deployment model. This is a public architectural overview, **not a customer installation guide**.

## Application Hosting

The application is designed to run from a customer-controlled Windows machine or server, with Windows Service hosting. Users access the supported Display, Operator, and Admin experiences through a browser.

## Local Access

Devices on an authorized local network can use the application through the configured host address, subject to the installation's network and access-control settings.

## Optional Remote Access

Customer environments may provide HTTPS access through an existing Cloudflare Tunnel configuration. External availability and access controls are deployment-specific.

This repository does not publish hostnames, database paths, customer-specific ports, credentials, installer scripts, or network configuration.

## Code & Configuration

Application source code, customer settings, and production configuration are private and excluded from this showcase.
