# Homewellness

![Homewellness overview](../assets/homewellness.svg)

A home healthcare marketplace connecting patients with providers. Its workflows cover service requests, quotations, appointments, provider verification, and administration.

[Visit the product](https://app.homewellnessplus.com/)

## Technology

Next.js · TypeScript · Hono · Bun · Drizzle ORM · PostgreSQL

## Product scope

- Patient + provider workflows
- Service requests + bookings
- Provider onboarding

## Workflow

```mermaid
flowchart LR
    A[Provider registration] --> B[Documents and service selection]
    B --> C[Admin review]
    C --> D[Provider available for bookings]
    E[Patient service request] --> F[Quotation or provider proposal]
    D --> F
    F --> G[Appointment confirmation]
    G --> H[Arrival verification]
    H --> I[Service completion and review]
```

## Engineering considerations

- Shared TypeScript contracts connect the API and dashboard.
- Hono services use Drizzle ORM with PostgreSQL.
- Patient, provider, and admin permissions govern booking and onboarding actions.
- Document review and provider approval gate availability for bookings.

This is a simplified product workflow based on the project documentation.

[Back to profile](../README.md)
