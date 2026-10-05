# Fashion E-Commerce Platform: Architecture

System design of a microservices e-commerce backend built by Kumar Suyash. The source code is in a private repository; this repository publishes only the architecture diagrams.

**Live site:** https://kumar-suyash.github.io/ecommerce-architecture/

## Status

Ten NestJS services behind one API gateway, in an Nx monorepo. Built and tested so far: the foundation, `auth-service`, `api-gateway`, `catalog-command`, `catalog-query` and `files-service` — 49 REST endpoints, 20 PostgreSQL tables over 12 migrations, and 823 test cases across 127 spec files. `order-service`, `payment-service`, `notification-service` and `cron-scheduler` are designed in LLDs and come next.

## Diagrams

- [System architecture](https://kumar-suyash.github.io/ecommerce-architecture/system-architecture.html)
- [Authentication service](https://kumar-suyash.github.io/ecommerce-architecture/auth-service.html)
- [Catalog and images: CQRS with cache invalidation](https://kumar-suyash.github.io/ecommerce-architecture/catalog-services.html)
- [Image upload and cache bust](https://kumar-suyash.github.io/ecommerce-architecture/catalog-invalidation.html)
- [Checkout sequence](https://kumar-suyash.github.io/ecommerce-architecture/checkout-sequence.html)
- [Payment confirmation sequence](https://kumar-suyash.github.io/ecommerce-architecture/payment-confirmation.html)
- [Order lifecycle](https://kumar-suyash.github.io/ecommerce-architecture/order-lifecycle.html)

Each diagram is a self-contained HTML page: open it in any browser, explore a node, follow a route, or export it.

## Stack

TypeScript, NestJS 11, Next.js 16, PostgreSQL 15 (Prisma 7), Redis 7, Sharp, Cloudflare R2, Nx, Jest, Playwright, GitHub Actions, Docker Compose.
