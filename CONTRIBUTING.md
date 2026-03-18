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
cd gpu && cmake -B build && cmake --build build && cd ..
go build -tags gpu .
go test ./...
```

If you don't have CUDA or OpenCL installed, the C library still builds with a CPU reference backend. The `-tags gpu` flag enables the compiled C library regardless of which GPU backends are available.

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
