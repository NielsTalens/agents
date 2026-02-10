# Agent Instructions

This is a Ruby project. When making changes, follow these rules strictly.

## Language & Style
- Use idiomatic Ruby
- Prefer clarity over cleverness
- Avoid metaprogramming unless explicitly requested
- Follow existing patterns and conventions in the codebase
- Do not reformat unrelated code

## Linting & Security (Required)
After any code change:
- Run `bundle exec rubocop` and fix all offenses
- Run `bundle exec brakeman` and address all high/medium warnings
- Do not suppress warnings unless explicitly justified in comments

If these tools fail, the change is incomplete.

## Tests
- Add or update tests when behavior changes
- Prefer minimal, focused tests
- Do not change existing tests unless they are incorrect or outdated
- All tests must pass before considering the task complete

## Dependencies
- Do not add new gems without explicit instruction
- Do not upgrade Ruby or gem versions unless asked
- Avoid expanding the dependency surface

## Security & Data Safety
- Treat all external input as untrusted
- Avoid dynamic evaluation (`eval`, `send`, `constantize`) unless unavoidable
- Prefer allowlists over denylists
- Do not log sensitive data

## Performance
- Avoid N+1 queries and unnecessary allocations
- Prefer explicit over implicit iteration
- Do not introduce premature optimization

## Documentation
- Update inline documentation when behavior changes
- Keep comments factual and minimal
- Do not restate obvious code

## Scope Control
- Make the smallest possible change to solve the problem
- Avoid refactors unless explicitly requested
- If a change has large blast radius, explain before proceeding

## Git discipline
- Write clear, imperative commit messages
- One logical change per commit- Fail loudly on programmer errors
- Handle user errors gracefully
- Avoid rescuing `StandardError` broadly


## Error handling


