# Architecture

Ürün360 is designed as a browser-based application backed by an ASP.NET Core Web API.

## Browser-Based Access

Users access the system through a browser. No traditional desktop client is required for end users.

## Local / Server-First Deployment

The application is intended to run on a local machine or an internal server. Devices on the same network can access the application through the server address.

## Windows Service Hosting

The backend hosts the application as a Windows Service. This allows the system to start automatically with Windows and stay available without manually running a console application.

## API-First Integration

The frontend communicates with the backend API. Product lookup, settings, health checks, and integration logic are handled through the API layer.

## Backend-Controlled Database Access

The frontend never connects directly to the database. Database access is controlled by the backend.

## Read-Only Database Access

Initial Wolvox Firebird integration is designed around a read-only principle. Product lookup and related information are retrieved without modifying the Wolvox database schema or customer data.

## Responsive Display

The display interface is designed for multiple screen sizes:

- TV and kiosk screens
- Cashier monitors
- Tablets
- Mobile phones

## Application Routes

### `/display`

Customer-facing or kiosk-style product display screen. It waits for barcode/QR input and shows the product clearly for a configurable duration.

### `/operator`

Staff-facing operation screen for barcode lookup, manual product search, product details, and operational modules.

### `/admin`

Configuration and management screen for display settings, scanner behavior, feature visibility, application configuration, and health checks.
