# Security

This public repository is documentation-only.

## Public Repository Rules

This repository does not contain:

- Source code
- Database credentials
- Environment files
- Application settings
- Customer-specific implementation details
- Wolvox database table or query details
- Private deployment configuration

## Database Access Principle

The frontend never connects directly to the database. Database access is handled by the backend API.

## Read-Only Principle

Initial Wolvox Firebird integration is designed with a read-only principle. Product information can be queried without modifying customer data or the Wolvox database schema.

## Risky Operations

Operations such as price updates, image upload, and label printing require additional validation, role-based authorization, auditability, and deployment-specific review before activation.

## Public IP Deployment

Public IP deployment requires a separate security review. HTTPS, authentication, firewall rules, rate limiting, and access control should be evaluated before exposing the application outside an internal network.
