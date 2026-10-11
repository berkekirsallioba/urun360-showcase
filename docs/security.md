# Security & Privacy

This repository is a **public, documentation-only showcase**. It does not include:

- Proprietary application source code
- Customer or employee records
- Database credentials, connection strings, or environment files
- Customer-specific settings or private deployment scripts
- ERP table definitions, private SQL queries, or internal implementation details

## Data Access Boundary

The browser interacts with the ASP.NET Core API; it does not directly connect to the Wolvox Firebird database.

The product has both information-lookup functionality and operational workflows for price and image changes. Earlier public documentation described the entire integration as read-only; that description is no longer accurate.

Authentication, authorization, validation, logging, and other protections must be reviewed in the context of the actual deployment. This showcase does **not** certify a specific customer's security posture.

## External Access

Some deployments can use HTTPS through a configured Cloudflare Tunnel. The existence of this option is not a claim that every installation is Internet-accessible or identically secured.

## Visuals

SVG previews in this repository are representative concepts, not live application screenshots. They do not contain customer data.
