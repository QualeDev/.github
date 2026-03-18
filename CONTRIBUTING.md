# Contributing to Quale

Thanks for your interest in contributing. Here's how to get started.

## Development workflow

We use **test-driven development (TDD)**. Every code change follows this cycle:

1. Write a failing test that describes the expected behaviour
2. Run it to confirm it fails
3. Write the minimum code to make it pass
4. Run tests to confirm it passes
5. Refactor if needed, keeping tests green
6. Commit

Pull requests without tests will be asked to add them.

## Getting started

```bash
git clone https://github.com/QualeDev/Engine.git
cd Engine
go test ./...
```

CI runs the full build (including GPU backends) on every push and pull request. You don't need CUDA or a GPU locally - just write and test your code, push it, and CI validates the complete build.

## Code style

- Follow existing patterns in the codebase
- Keep files focused and under ~500 lines
- Document public APIs with doc comments
- Comments explain *why*, not *what*
- No comments referencing migrations, rewrites, or previous implementations

## Pull requests

- One logical change per PR
- Write a clear title and description
- Fill out the PR template checklist
- Ensure `go test ./...` passes before submitting

## Reporting bugs

Use the [bug report template](https://github.com/QualeDev/Engine/issues/new?template=bug_report.yml) with steps to reproduce and your `.quale` file if relevant.

## Questions

Check the [documentation](https://quale.dev/docs/) first. If you're still stuck, open a [question issue](https://github.com/QualeDev/Engine/issues/new?template=question.yml).
