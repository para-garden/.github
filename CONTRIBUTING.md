# Contributing

Guidelines for contributing to para-garden projects.

## Development Setup

Projects vary in their tech stacks. Check each project's README for specific setup instructions.

### Nix (Optional)

For reproducible environments, projects include `flake.nix`:

```bash
nix develop
# or with direnv: direnv allow
```

This ensures exact versions of all dependencies but isn't required.

## Commit Conventions

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
type(scope): description

[optional body]
```

Types:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation only
- `refactor`: Code change that neither fixes a bug nor adds a feature
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

Examples:
```
feat(rooms): add room transition system
fix(input): prevent double-submit on enter
docs(guide): document game mechanics
```

## Pull Requests

1. Fork the repository
2. Create a feature branch from `master`
3. Make your changes with conventional commits
4. Ensure checks pass
5. Open a PR with a clear description

## Documentation

Each project has a `docs/` directory with VitePress:

```bash
cd docs
bun install
bun run dev
```

When adding features, update relevant documentation. Prefer updating existing docs over creating new files.

## Questions?

Open an issue in the relevant repository.
