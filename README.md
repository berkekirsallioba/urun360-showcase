<p align="center">
  <img src="./assets/logo.png" width="160" alt="Ürün360 logo" />
</p>

<h1 align="center">Ürün360</h1>
<p align="center"><strong>ERP-Integrated Product Lookup & Price Display Platform</strong></p>
<p align="center">Barcode / QR scanning · Product information · Retail operations</p>

> **Public portfolio showcase only.** Application source code, customer data, database details, and private deployment configuration are not published here.

## The Business Problem

Retail and warehouse teams need quick access to reliable product information at the point of service. Product details may live in an ERP system, while employees and customers need a clear, responsive experience on cashier displays, kiosks, tablets, and phones.

**Ürün360** bridges that workflow with a browser-based interface connected to **AKINSOFT Wolvox ERP** data through a **C# / ASP.NET Core backend**.

## What Ürün360 Does

- Looks up products through barcode and QR-based workflows.
- Displays product names, prices, stock information, and other available product details.
- Supports multiple price presentations and product imagery.
- Offers separate browser-based **Display**, **Operator**, and **Admin** experiences.
- Includes operational workflows for **product price updates** and **product image changes**, in addition to information display.
- Runs in a server-first model, with browser access from supported client devices.

Feature availability and behavior depend on the application version and customer configuration. This showcase is not a public live demo.

## Application Experiences

### Display — Customer-Facing Product Information

Designed for visible product identification and price presentation on customer displays, kiosks, and other screens.

![Representative Display concept](./assets/screenshots/display-mode.svg)

### Operator — Staff Product Operations

Supports product lookups and staff-facing product information and operational workflows.

![Representative Operator concept](./assets/screenshots/operator-mode.svg)

### Admin — Configuration

Provides an administrative surface for supported configuration and application settings.

![Representative Admin concept](./assets/screenshots/admin-mode.svg)

**Visual note:** The three images above are illustrative SVG mockups, **not screenshots of the live application**. They contain no customer information.

## Technology Overview

| Area | Technologies |
| --- | --- |
| Backend | C#, .NET, ASP.NET Core Web API |
| Frontend | React, TypeScript |
| Data integration | AKINSOFT Wolvox ERP, Firebird |
| Deployment approach | Windows Service / local-server hosting, browser-based access |
| External access | HTTPS through an appropriately configured Cloudflare Tunnel deployment |

The application interface communicates with the backend API; the browser does not directly connect to the ERP database.

### High-Level Architecture

```text
Barcode / QR input or product search
                 |
          Browser interface
      Display / Operator / Admin
                 |
        ASP.NET Core Web API
                 |
       Wolvox ERP / Firebird
```

This is intentionally a simplified conceptual diagram; internal schemas, queries, customer-specific settings, and proprietary implementation details are excluded.

## Engineering Focus

- Connecting a modern browser interface to an existing ERP data source
- Designing product lookup and information-display workflows for different devices
- Handling product pricing, stock visibility, and operational data changes
- Separating customer-facing, operator, and administrative experiences
- Supporting a locally hosted application with optional secure remote access

## Ongoing Improvements

The product continues to evolve. Current areas of refinement include:

- Display layout for long product names and more prominent secondary prices
- Fast product search across names, codes, and barcode/QR input
- Consistent spoken-price behavior on mobile devices

These are **improvement areas**, not claims that every enhancement has already been completed or deployed.

## Source Code & Privacy

This repository contains **presentation documentation and representative visuals only**.

The application source code remains private. Customer records, credentials, Firebird database schemas, private deployment scripts, and configuration secrets are not shared.

See [Security & privacy](./docs/security.md) and [Repository notice](./NOTICE.md).

## About the Developer

Created as part of my work building enterprise software and ERP-integrated business applications.

**Berke Kırşallıoba** — Full-Stack .NET Developer

[GitHub Profile](https://github.com/berkekirsallioba) · [LinkedIn](https://www.linkedin.com/in/berkekirsallioba)
