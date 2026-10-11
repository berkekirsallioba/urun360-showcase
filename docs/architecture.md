# Architecture

Ürün360 is a browser-based application with a React / TypeScript interface and an ASP.NET Core backend API connected to Wolvox ERP / Firebird data.

## Browser-Based Access

Users interact through a web browser rather than a traditional desktop client. The application has distinct Display, Operator, and Admin experiences.

## Local / Server-First Deployment

The application is intended to run on a local machine or customer-managed server, with Windows Service hosting. Supported devices can access the application through a browser.

## Integration Boundary

The browser communicates with the backend API. The backend handles ERP data access; database credentials and customer-specific connection details are not exposed to clients.

## Data Operations

The product supports product information lookups and operational workflows that include product price updates and product image changes. It must **not** be represented as a universally read-only application.

Exact write paths, authorization rules, ERP table structures, and customer-specific safeguards are intentionally omitted from this public description.

## High-Level Flow

```text
Barcode / QR input or product search
                 ↓
         Browser interface
    Display / Operator / Admin
                 ↓
       ASP.NET Core API
                 ↓
       Wolvox ERP / Firebird
```

## Representative Visuals

The public showcase SVGs are illustrative mockups, not screenshots or evidence of a particular live deployment.
