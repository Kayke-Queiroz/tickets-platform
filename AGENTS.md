# Tickets Platform - Project Guidelines & Context

## Project Description
A modular monolith ticketing platform built with NestJS.

## Tech Stack
- **Framework:** NestJS
- **Language:** TypeScript (strict mode)
- **Database / ORM:** PostgreSQL 16, Prisma ORM
- **Testing:** Vitest / Jest

## Git Commit Standard
- Strictly follow **Conventional Commits** in English:
  - `feat:` A new feature
  - `fix:` A bug fix
  - `chore:` Maintenance, configuration, dependencies
  - `test:` Adding or refactoring tests
  - `docs:` Documentation changes

## Code Guidelines
- **Language:** Code, identifiers, and comments must be strictly in English. Portuguese is allowed only for public domain/business text/messages if necessary.
- **Modular Monolith Architecture:** Modules are isolated by business domain inside `src/modules/`:
  - `auth`
  - `events`
  - `orders`
  - `payments`
  - `tickets`
- **Validation:** Use `class-validator` and `class-transformer` for DTOs.
- **Type Safety:** Explicit return types for all methods and functions (no `any`).

## Frequent Commands
- **Start Database:** `docker compose up -d`
- **Start Development Server:** `npm run start:dev`
- **Type Check:** `npx tsc --noEmit`
- **Linter:** `npm run lint`
- **Unit Tests:** `npm test`
