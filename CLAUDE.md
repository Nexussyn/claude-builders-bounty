# Fix for Issue #2: [BOUNTY $75] TEMPLATE: CLAUDE.md for a Next.js + SQLite SaaS project

# Stack & Versions
* Next.js: 15
* SQLite: better-sqlite3
* Node.js: 18.x

# Folder Structure
* `components`: Reusable React components
* `containers`: Page-level components
* `db`: Database schema and migration files
* `lib`: Utility functions
* `pages`: Next.js pages
* `public`: Static assets
* `styles`: Global CSS styles

# SQL / Migration Conventions
* Use `better-sqlite3` for database interactions
* Migrations are stored in `db/migrations`
* Migration files follow the format `YYYYMMDDHHMMSS_description.sql`
* Use `sqlite3` command-line tool for database inspection and debugging

# Component Patterns
* Use functional components with hooks
* Keep components small and focused on a single task
* Use `React.memo` for memoization when necessary
* Avoid using `index.js` files; instead, use explicit file names

# What we don't do (and why)
* We don't use class components; instead, we use functional components with hooks for better performance and easier debugging.
* We don't use inline styles; instead, we use global CSS styles in `styles` folder for better maintainability.
* We don't commit large files; instead, we use external storage services like AWS S3 for storing large assets.

# Dev Commands
* `npm run dev`: Start the development server
* `npm run build`: Build the production bundle
* `npm run migrate`: Run database migrations
* `npm run test`: Run unit tests and integration tests

# Patterns to Follow
* Keep code organized and modular
* Use meaningful variable names and function names
* Use comments to explain complex logic
* Avoid duplicated code; instead, extract reusable functions or components