# Contributing to Necromancer Labs

We welcome contributions from the security research community.

## Before You Start

1. Check existing issues to avoid duplicating work
2. For major changes, open an issue first to discuss the approach
3. Ensure your work aligns with the project's goals

## Pull Request Process

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Write clear, focused commits
4. Test your changes on relevant target architectures
5. Submit a pull request with a clear description

## Code Standards

- Keep it simple. Embedded targets have constraints.
- Avoid unnecessary dependencies
- Document non-obvious behavior
- Include target architecture compatibility notes where relevant

## Testing

If adding functionality:
- Test on at least one real or emulated target
- Note which architectures you tested against
- Include reproduction steps for any bugs fixed

## Commit Messages

Write clear commit messages that explain *what* and *why*:

```
Add MIPS big-endian support for flash extraction

The existing implementation assumed little-endian byte order.
This breaks on older Broadcom-based routers. Fixed by detecting
endianness from ELF headers at runtime.
```

## Questions?

Open an issue or reach out. We're here to help serious contributors.
