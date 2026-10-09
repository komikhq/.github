# Organization-Wide Copilot Instructions

These instructions define the architectural, styling, and coding standards across all repositories in the **KomikHQ** organization.

---

## Architectural Principles

1. **Edge-First and Serverless**:
   - Target Cloudflare Workers and modern edge runtimes where applicable.
   - Rely on web standard APIs (`Request`, `Response`, `Fetch API`, `Streams`) rather than Node.js-specific modules (`fs`, `net`, `child_process`).
   - Use Hono for lightweight, type-safe API routing.

2. **Frontend Architecture**:
   - Use Astro for content-driven and layout layers with zero-JS by default.
   - Use React 19 for interactive islands requiring stateful client operations.
   - Use Tailwind CSS v4 without redundant abstractions.

3. **Database and ORM**:
   - Neon Serverless PostgreSQL with connection pooling.
   - Drizzle ORM for schema definition and migrations. Keep queries explicit, type-safe, and avoid N+1 query patterns.

---

## TypeScript and Code Quality Standards

1. **Strict Type Safety**:
   - `strict: true` is enabled across all codebases.
   - Never use `any`. Use `unknown` with type narrowing, generics, or schemas (e.g., Zod) instead.
   - Prefer explicit return types on public functions, API handlers, and exported interfaces.

2. **Error Handling**:
   - Return structured error responses with HTTP status codes matching RFC conventions.
   - Avoid silent try/catch blocks. Propagate errors or log with contextual detail.

3. **Style and Syntax**:
   - Use ES Modules (`import`/`export`) exclusively.
   - Use arrow functions for callbacks and named function declarations for top-level component/service exports.
   - Maintain concise, readable, and self-documenting code. Do not include unnecessary comments explaining trivial operations.
