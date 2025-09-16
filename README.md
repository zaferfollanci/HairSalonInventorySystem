# Hair Salon Inventory System

A modern, production-ready, containerized inventory solution for hair salons.

## Features

- Stock Movements (entries/exits, categories)
- Dashboard & Analytics (charts, filters)
- Notifications (in-app, email, SignalR)
- User Authentication & Role-based Access (Identity, JWT)
- Barcode/QR Support (scan/search)
- Multi-language (EN/TR, dynamic switching)
- Supplier/Branch/Sales/Expense Management
- Audit Log (user actions, filtering)
- Docker Compose, CI/CD, Tests

## Quick Start (Docker)

```bash
docker-compose up --build
```
- API: http://localhost:5000
- Blazor: http://localhost:5002
- DB: localhost:5432 (user: hsadmin / pass: strongpassword / db: hairsalon)

## Running Tests

```bash
dotnet test src/HairSalonInventory.Tests
```

## Notes

- Configure environment variables for production (`docker-compose.yml`)
- Use your own secrets for JWT and DB
- For multi-language, see `src/HairSalonInventory.Blazor/Resources/`