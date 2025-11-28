# Project Guidelines

## Commit Format

Use conventional commits: `type(scope): description`

Types:
- `feat` - new feature
- `fix` - bug fix
- `refactor` - code restructuring without behavior change
- `chore` - maintenance tasks, dependencies, config
- `docs` - documentation only
- `style` - formatting, no code change
- `test` - adding or updating tests

## Code Organization

### Small Modular Files
- Keep files focused on a single responsibility
- Extract reusable logic into separate modules
- Aim for files under 150 lines when practical

### Separation of Concerns
- Components handle UI rendering only
- Business logic goes in dedicated utility modules
- Keep styles scoped to their components
- Data fetching separate from presentation

### File Structure
```
src/
├── components/    # Reusable UI components
├── layouts/       # Page layouts
├── pages/         # Route pages
├── utils/         # Helper functions
├── types/         # TypeScript types
└── styles/        # Global styles (if needed)
```

## Astro Conventions

- Use `.astro` for static components
- Use framework components (React/Vue/Svelte) only when interactivity is needed
- Prefer static rendering over client-side JavaScript
- Use content collections for structured content
